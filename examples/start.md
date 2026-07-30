---
layout: default
title: Start page example
permalink: /examples/start/
hide_service_nav: true
---

<nav class="govuk-breadcrumbs" aria-label="Breadcrumb">
  <ol class="govuk-breadcrumbs__list">
    <li class="govuk-breadcrumbs__list-item">
      <a class="govuk-breadcrumbs__link" href="{{ site.baseurl }}/">Home</a>
    </li>
    <li class="govuk-breadcrumbs__list-item">
      <a class="govuk-breadcrumbs__link" href="#">Section</a>
    </li>
    <li class="govuk-breadcrumbs__list-item">
      Subsection
    </li>
  </ol>
</nav>

<div class="govuk-grid-row">
  <div class="govuk-grid-column-two-thirds">

    <h1 class="govuk-heading-xl">{{ site.title }}</h1>

    <p class="govuk-body">Use this service to:</p>

    <ul class="govuk-list govuk-list--bullet">
      <li>do something</li>
      <li>update your name, address or other details</li>
      <li>do something else</li>
    </ul>

    <p class="govuk-body">Registering takes around 5 minutes.</p>

    <a href="{{ site.baseurl }}/examples/question/" role="button" draggable="false" class="govuk-button govuk-button--start govuk-!-margin-top-2 govuk-!-margin-bottom-8" data-module="govuk-button">
      Start now
      <svg class="govuk-button__start-icon" xmlns="http://www.w3.org/2000/svg" width="17.5" height="19" viewBox="0 0 33 40" aria-hidden="true" focusable="false">
        <path fill="currentColor" d="M0 0h13l20 20-20 20H0l20-20z"></path>
      </svg>
    </a>

    <h2 class="govuk-heading-m">Before you start</h2>

    <p class="govuk-body">You can also <a class="govuk-link" href="#">register by post</a>.</p>

    <p class="govuk-body">The online service is also available in <a class="govuk-link" href="#">Welsh (Cymraeg)</a>.</p>

    <p class="govuk-body">You can't register for this service if you're in the UK illegally.</p>

  </div>

  <div class="govuk-grid-column-one-third">
    <aside role="complementary">
      <h2 class="govuk-heading-m" id="subsection-title">
        Subsection
      </h2>
      <nav role="navigation" aria-labelledby="subsection-title">
        <ul class="govuk-list govuk-body-s">
          <li><a class="govuk-link" href="#">Related link</a></li>
          <li><a class="govuk-link" href="#">Related link</a></li>
          <li><a class="govuk-link govuk-!-font-weight-bold" href="#">More <span class="govuk-visually-hidden">in Subsection</span></a></li>
        </ul>
      </nav>
    </aside>
  </div>
</div>
