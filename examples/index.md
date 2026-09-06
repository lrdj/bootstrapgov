---
layout: default
title: Examples
permalink: /examples/
---

<div class="govuk-grid-row">
  <div class="govuk-grid-column-two-thirds">

    <h1 class="govuk-heading-xl">Example pages</h1>

    <p class="govuk-body">These are working example pages built with GOV.UK Frontend. The first four link together as a complete journey, from start page to confirmation. Duplicate any of these files in <code class="govuk-!-font-size-16">examples/</code> to start a new page.</p>

    {%- assign example_pages = site.pages | where_exp: "p", "p.url contains '/examples/'" | where_exp: "p", "p.url != '/examples/'" | sort: "order" -%}

    <ul class="govuk-list govuk-list--spaced">
      {%- for p in example_pages %}
      <li>
        <a class="govuk-link govuk-!-font-weight-bold" href="{{ site.baseurl }}{{ p.url }}">{{ p.title }}</a>
        {%- if p.description %}
        <br><span class="govuk-body-s govuk-!-margin-bottom-0">{{ p.description }}</span>
        {%- endif %}
      </li>
      {%- endfor %}
    </ul>

    <p class="govuk-body">To add a page to this list, put <code class="govuk-!-font-size-16">order:</code> and <code class="govuk-!-font-size-16">description:</code> in its front matter. Pages without an order appear at the end.</p>

  </div>
</div>
