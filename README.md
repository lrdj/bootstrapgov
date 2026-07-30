# Bootstrap govuk

A GOV.UK-styled prototype you can preview locally and publish for free with GitHub Pages — no Heroku account, no Node server, no deploy pipeline to get past IT.

## Why this exists

The [GOV.UK Prototype Kit](https://prototype-kit.service.gov.uk/) is the standard tool for prototyping GOV.UK services, but sharing a kit prototype usually means deploying it somewhere — traditionally Heroku, sometimes another Node host. If you're working somewhere that won't let you sign up for Heroku, doesn't allow outbound Node deployments, or you just don't want to deal with a server at all, that's a hard blocker.

This repo is the workaround. It's a plain [Jekyll](https://jekyllrb.com/) site — Jekyll turns simple text files into static HTML pages, and GitHub will host and rebuild it for you automatically every time you push, for free, at a `github.io` URL. There's no server to manage, no account to request access to, nothing running that can go down. You write pages, push to `main`, and GitHub Pages does the rest.

It uses the **real, current [GOV.UK Frontend](https://frontend.design-system.service.gov.uk/)** — the same CSS and JS that powers the actual Prototype Kit and real GOV.UK services — so anything you build here looks and behaves exactly as it would in the kit. It's not a lookalike.

## What's different from the kit (read this first)

This is the trade-off for not needing a server:

- **No forms that submit anywhere.** The kit uses Node routes to handle form submissions, store session data, and branch between pages based on answers. This site can't do any of that — it's just HTML files. Buttons that would submit a form in the kit are plain links here, styled to look identical.
- **No session data / "answers so far".** You can't show a user's own input back to them (`{{ data['question'] }}` style patterns don't exist here).
- **You can still fake a journey.** Pages can link to each other in order, so a start page → question → check your answers → confirmation flow still *feels* like a real service, even though nothing is actually being submitted or stored. See `examples/` below — that's a working example of exactly this.

If you need real form logic, session data, or branching, this isn't a substitute for the kit — it's specifically for the situation where you need something GOV.UK-shaped to look at or share, and running the kit properly isn't an option.

## "I need routes.js" — what to do instead

In the kit, `app/routes.js` is where you'd write server logic: show a different next page depending on what someone answered, remember their answers, call an API, that sort of thing. There's no equivalent here, because there's no server — so if you're reaching for routes.js, first check which of these you actually need:

- **"Show a different page depending on the answer"** — you don't necessarily need real branching for this, you can *fake* it. Build both outcomes as separate static pages (`confirmation-eligible.md`, `confirmation-not-eligible.md`) and link each answer straight to the page it leads to. Zero JavaScript, and stakeholders clicking through genuinely can't tell the difference.
- **"Remember an answer and use it on a later page"** (redirect based on a previous answer, populate a check-your-answers page with what someone actually typed) — this doesn't need a server either. "Static site" only means no server-side computation; it says nothing about JavaScript running in the browser. A small script using `localStorage` can save an answer on one page and read it back on the next, entirely client-side, and GitHub Pages serves it exactly the same as any other file. This is a good thing to ask an LLM for directly — describe the pages and what should carry over between them, and ask for a vanilla JS snippet using `localStorage` (no build step, no framework). Good enough for demos and usability testing; not real data storage, and answers won't survive someone clearing their browser data or switching devices.
- **"I actually need a real backend"** — an API call needing a secret key, data that has to persist across devices or for other people to see, anything that genuinely can't run in one person's browser — there's no way round this without a Node server somewhere. Worth trying, roughly in order of effort:
  1. Ask specifically for Heroku (or equivalent) access for this one project, rather than general hosting access — it's a much narrower, easier ask than it sounds, and this is exactly the kind of case that justifies it.
  2. Run the real Prototype Kit **locally only** — you get full routes.js logic on your own machine, and share it as a screen recording or in a review session rather than a live link. Nothing to deploy, nothing to get sign-off for.
  3. Look at free Node hosts that aren't Heroku (Glitch and Render both have free tiers as of writing) in case your organisation's block is Heroku-specific rather than blanket — worth a quick check with IT before assuming it's a dead end.

## Getting started

You'll need Ruby installed (check with `ruby -v` in Terminal — if that fails, install via [rbenv](https://github.com/rbenv/rbenv) or similar). Then, from this folder:

```
bundle install
bundle exec jekyll serve
```

This starts a local preview server. Because the site is configured to eventually live at `github.io/bootstrapgov`, your local preview mirrors that — visit **`http://localhost:4000/bootstrapgov/`** (note the trailing path, it's easy to miss and land on a blank page without it).

Leave `jekyll serve` running in a terminal window while you work — it rebuilds automatically every time you save a file, so you just refresh the browser to see changes.

## Where things live

| Folder / file | What it's for |
|---|---|
| `index.md`, `gov.md`, `component-test.md`, `examples/*.md` | **The actual pages.** Each one is mostly plain HTML with a short header block (front matter) on top. This is where you'll spend your time. |
| `_layouts/default.html` | The page "frame" — GOV.UK header, footer, skip link — wrapped around every page's content. You shouldn't need to touch this. |
| `_includes/` | Small reusable snippets (like the service navigation bar) pulled into layouts. |
| `assets/govuk/` | The vendored GOV.UK Frontend package — the CSS/JS that makes everything look and behave like GOV.UK. Don't edit inside here; it gets replaced wholesale when the version is upgraded. |
| `_config.yml` | Site-wide settings — the service name (`title:`) shown in the header, and the `baseurl` GitHub Pages needs (see below — don't touch this unless you know why). |

## Adding a new page

Create a new `.md` file anywhere in the project (or in `examples/` alongside the existing ones) with this at the top:

```
---
layout: default
title: My new page
permalink: /my-new-page/
---
```

Then write or paste your HTML underneath, with a blank line separating it from the block above. That's the whole recipe — Jekyll handles the rest.

## Pulling components straight from the Design System

This is the main trick worth knowing: you can go to the [GOV.UK Design System](https://design-system.service.gov.uk/components/), find a component (breadcrumbs, buttons, radios, whatever), copy the **HTML example** shown on that page, and paste it directly into one of this site's `.md` files. It'll just work — same classes, same CSS, same JS behaviour, because this site runs the same version of GOV.UK Frontend.

Two things to watch for when pasting:
1. Copy from the **"HTML" example code panel**, not the whole page — grabbing more than that can pull in the design system website's own extra wrapper markup, which isn't part of GOV.UK Frontend and won't do anything useful here.
2. If a component has an `id` (form fields, mostly) and you paste more than one copy onto the same page, make the ids unique by hand — duplicate ids are the one thing that'll genuinely break.

`component-test.md` in this repo is a working reference — it's a single page with one of nearly every component, copied straight from the vendored package, so you can see what "correctly pasted" looks like and copy the pattern.

## The example journey

`examples/start.md` → `question.md` → `check-your-answers.md` → `confirmation.md` is a small working demo of a typical GOV.UK service flow, click-through-able end to end. It's a good starting template if you're mocking up a real journey — duplicate these files and edit the content rather than starting from a blank page.

## Publishing

```
git add .
git commit -m "your message"
git push
```

Once pushed to `main`, GitHub rebuilds and republishes the site automatically — no separate deploy step, no dashboard to click through. Give it a minute or two after pushing before checking the live URL.

## The one setting not to touch: `baseurl`

In `_config.yml`:

```yaml
baseurl: "/bootstrapgov"
```

GitHub Pages serves this repo at `https://<username>.github.io/bootstrapgov/` — the repo name becomes part of the URL. Every link and asset on the site is built around that path, and it's also why your local preview lives at `localhost:4000/bootstrapgov/` rather than the plain root. If you ever rename the GitHub repo, this value needs to change to match — otherwise leave it alone.
