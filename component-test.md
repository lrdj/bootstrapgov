---
layout: default
title: Design system component test
permalink: /component-test/
---

<span class="govuk-caption-l">GOV.UK Frontend</span>
<h1 class="govuk-heading-xl">Component test page</h1>
<p class="govuk-body">Every component below is copied unmodified from the <code class="govuk-!-font-size-16">assets/govuk/components/&lt;name&gt;/template-default.html</code> examples that ship inside the govuk-frontend package, so this page doubles as a check that the vendored version (currently <strong class="govuk-tag">6.4.0</strong>) still renders and behaves correctly.</p>

<hr class="govuk-section-break govuk-section-break--l govuk-section-break--visible">

<h2 class="govuk-heading-l">Back link</h2>
<a href="#" class="govuk-back-link">Back</a>

<hr class="govuk-section-break govuk-section-break--l govuk-section-break--visible">

<h2 class="govuk-heading-l">Typography</h2>
<span class="govuk-caption-m">govuk-caption-m</span>
<h2 class="govuk-heading-l">govuk-heading-xl / heading-l</h2>
<h3 class="govuk-heading-m">govuk-heading-m</h3>
<h4 class="govuk-heading-s">govuk-heading-s</h4>
<p class="govuk-body-l">govuk-body-l — Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
<p class="govuk-body">govuk-body — Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore.</p>
<p class="govuk-body-s">govuk-body-s — Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
<ul class="govuk-list govuk-list--bullet">
  <li>govuk-list--bullet item one</li>
  <li>govuk-list--bullet item two</li>
</ul>
<ul class="govuk-list govuk-list--number">
  <li>govuk-list--number item one</li>
  <li>govuk-list--number item two</li>
</ul>
<a class="govuk-link" href="#">govuk-link default link style</a>

<hr class="govuk-section-break govuk-section-break--l govuk-section-break--visible">

<h2 class="govuk-heading-l">Grid</h2>
<div class="govuk-grid-row">
  <div class="govuk-grid-column-two-thirds">
    <p class="govuk-body">govuk-grid-column-two-thirds</p>
  </div>
  <div class="govuk-grid-column-one-third">
    <p class="govuk-body">govuk-grid-column-one-third</p>
  </div>
</div>

<hr class="govuk-section-break govuk-section-break--l govuk-section-break--visible">

<h2 class="govuk-heading-l">Buttons</h2>
<div class="govuk-button-group">
  <button type="submit" class="govuk-button" data-module="govuk-button">
    Save and continue
  </button>
  <button type="submit" name="secondary" class="govuk-button govuk-button--secondary" data-module="govuk-button">
    Secondary button
  </button>
  <button type="submit" name="Warning" class="govuk-button govuk-button--warning" data-module="govuk-button">
    Warning button
  </button>
  <button type="submit" disabled aria-disabled="true" class="govuk-button" data-module="govuk-button">
    Disabled button
  </button>
</div>
<a class="govuk-button govuk-button--start" href="#" data-module="govuk-button">Start now <svg class="govuk-button__start-icon" xmlns="http://www.w3.org/2000/svg" width="17.5" height="19" viewBox="0 0 33 40" aria-hidden="true" focusable="false"><path fill="currentColor" d="M0 0h13l20 20-20 20H0l20-20z" /></svg></a>

<hr class="govuk-section-break govuk-section-break--l govuk-section-break--visible">

<h2 class="govuk-heading-l">Tags</h2>
<p class="govuk-body">Checking the v6 colour renames (pink&nbsp;&rarr;&nbsp;magenta, turquoise&nbsp;&rarr;&nbsp;teal) render correctly.</p>
<p>
  <strong class="govuk-tag">Default (blue)</strong>
  <strong class="govuk-tag govuk-tag--grey">Grey</strong>
  <strong class="govuk-tag govuk-tag--green">Green</strong>
  <strong class="govuk-tag govuk-tag--red">Red</strong>
  <strong class="govuk-tag govuk-tag--yellow">Yellow</strong>
  <strong class="govuk-tag govuk-tag--orange">Orange</strong>
  <strong class="govuk-tag govuk-tag--purple">Purple</strong>
  <strong class="govuk-tag govuk-tag--magenta">Magenta</strong>
  <strong class="govuk-tag govuk-tag--teal">Teal</strong>
</p>

<hr class="govuk-section-break govuk-section-break--l govuk-section-break--visible">

<h2 class="govuk-heading-l">Panel</h2>
<div class="govuk-panel govuk-panel--confirmation">
  <h1 class="govuk-panel__title">
    Application complete
  </h1>
  <div class="govuk-panel__body">
    Your reference number<br><strong>HDJ2123F</strong>
  </div>
</div>

<hr class="govuk-section-break govuk-section-break--l govuk-section-break--visible">

<h2 class="govuk-heading-l">Notification banner</h2>
<div class="govuk-notification-banner" role="region" aria-labelledby="govuk-notification-banner-title" data-module="govuk-notification-banner">
  <div class="govuk-notification-banner__header">
    <h2 class="govuk-notification-banner__title" id="govuk-notification-banner-title">
      Important
    </h2>
  </div>
  <div class="govuk-notification-banner__content">
    <p class="govuk-notification-banner__heading">
      This publication was withdrawn on 7 March 2014.
    </p>
  </div>
</div>
<br>
<div class="govuk-notification-banner govuk-notification-banner--success" role="alert" aria-labelledby="govuk-notification-banner-title-success" data-module="govuk-notification-banner">
  <div class="govuk-notification-banner__header">
    <h2 class="govuk-notification-banner__title" id="govuk-notification-banner-title-success">
      Success
    </h2>
  </div>
  <div class="govuk-notification-banner__content">
    <p class="govuk-notification-banner__heading">
      Email sent to example@email.com
    </p>
  </div>
</div>

<hr class="govuk-section-break govuk-section-break--l govuk-section-break--visible">

<h2 class="govuk-heading-l">Warning text</h2>
<div class="govuk-warning-text">
  <span class="govuk-warning-text__icon" aria-hidden="true">!</span>
  <strong class="govuk-warning-text__text">
    <span class="govuk-visually-hidden">Warning</span>
    You can be fined up to £5,000 if you don’t register.
  </strong>
</div>

<h2 class="govuk-heading-l">Inset text</h2>
<div class="govuk-inset-text">
  It can take up to 8 weeks to register a lasting power of attorney if there are no mistakes in the application.
</div>

<hr class="govuk-section-break govuk-section-break--l govuk-section-break--visible">

<h2 class="govuk-heading-l">Details</h2>
<details class="govuk-details">
  <summary class="govuk-details__summary">
    <span class="govuk-details__summary-text">
      Help with nationality
    </span>
  </summary>
  <div class="govuk-details__text">
    We need to know your nationality so we can work out which elections you’re entitled to vote in. If you can’t provide your nationality, you’ll have to send copies of identity documents through the post.
  </div>
</details>

<hr class="govuk-section-break govuk-section-break--l govuk-section-break--visible">

<h2 class="govuk-heading-l">Error summary</h2>
<div class="govuk-error-summary" data-module="govuk-error-summary">
  <div role="alert">
    <h2 class="govuk-error-summary__title">
      There is a problem
    </h2>
    <div class="govuk-error-summary__body">
        <ul class="govuk-list govuk-error-summary__list">
          <li>
            <a href="#example-error-1">The date your passport was issued must be in the past</a>
          </li>
          <li>
            <a href="#example-error-2">Enter a postcode, like AA1 1AA</a>
          </li>
        </ul>
    </div>
  </div>
</div>

<hr class="govuk-section-break govuk-section-break--l govuk-section-break--visible">

<h2 class="govuk-heading-l">Form elements</h2>

<div class="govuk-form-group">
  <label class="govuk-label" for="test-name">
    National Insurance number
  </label>
  <input class="govuk-input" id="test-name" name="test-name" type="text">
</div>

<div class="govuk-form-group">
  <label class="govuk-label" for="more-detail-textarea">
    Can you provide more detail?
  </label>
  <textarea class="govuk-textarea" id="more-detail-textarea" name="more-detail-textarea" rows="5"></textarea>
</div>

<div class="govuk-form-group govuk-character-count" data-module="govuk-character-count" data-maxlength="10">
  <label class="govuk-label" for="more-detail">
    Character count — can you provide more detail?
  </label>
  <textarea class="govuk-textarea govuk-js-character-count" id="more-detail" name="more-detail" rows="5" aria-describedby="more-detail-info"></textarea>
  <div id="more-detail-info" class="govuk-hint govuk-character-count__message">
    You can enter up to 10 characters
  </div>
</div>

<div class="govuk-form-group">
  <label class="govuk-label" for="select-1">
    Label text goes here
  </label>
  <select class="govuk-select" id="select-1" name="select-1">
    <option value="1">GOV.UK frontend option 1</option>
    <option value="2" selected>GOV.UK frontend option 2</option>
    <option value="3" disabled>GOV.UK frontend option 3</option>
  </select>
</div>

<div class="govuk-form-group govuk-password-input" data-module="govuk-password-input">
  <label class="govuk-label" for="password">
    Password
  </label>
  <div class="govuk-input__wrapper govuk-password-input__wrapper">
    <input class="govuk-input govuk-password-input__input govuk-js-password-input-input" id="password" name="password" type="password" spellcheck="false" autocomplete="current-password" autocapitalize="none">
    <button type="button" class="govuk-button govuk-button--secondary govuk-password-input__toggle govuk-js-password-input-toggle" data-module="govuk-button" aria-controls="password" aria-label="Show password" hidden>
      Show
    </button>
  </div>
</div>

<div class="govuk-form-group">
  <label class="govuk-label" for="file-upload-1">
    Upload a file
  </label>
  <input class="govuk-file-upload" id="file-upload-1" name="file-upload-1" type="file">
</div>

<div class="govuk-form-group">
  <fieldset class="govuk-fieldset">
  <legend class="govuk-fieldset__legend">
    What is your nationality?
  </legend>
  <div class="govuk-checkboxes" data-module="govuk-checkboxes">
    <div class="govuk-checkboxes__item">
      <input class="govuk-checkboxes__input" id="nationality" name="nationality" type="checkbox" value="british">
      <label class="govuk-label govuk-checkboxes__label" for="nationality">
        British
      </label>
    </div>
    <div class="govuk-checkboxes__item">
      <input class="govuk-checkboxes__input" id="nationality-2" name="nationality" type="checkbox" value="irish">
      <label class="govuk-label govuk-checkboxes__label" for="nationality-2">
        Irish
      </label>
    </div>
    <div class="govuk-checkboxes__item">
      <input class="govuk-checkboxes__input" id="nationality-3" name="nationality" type="checkbox" value="other">
      <label class="govuk-label govuk-checkboxes__label" for="nationality-3">
        Citizen of another country
      </label>
    </div>
  </div>
</fieldset>
</div>

<div class="govuk-form-group">
  <fieldset class="govuk-fieldset">
  <legend class="govuk-fieldset__legend">
    Have you changed your name?
  </legend>
  <div class="govuk-radios" data-module="govuk-radios">
    <div class="govuk-radios__item">
      <input class="govuk-radios__input" id="example-default" name="example-default" type="radio" value="yes">
      <label class="govuk-label govuk-radios__label" for="example-default">
        Yes
      </label>
    </div>
    <div class="govuk-radios__item">
      <input class="govuk-radios__input" id="example-default-2" name="example-default" type="radio" value="no">
      <label class="govuk-label govuk-radios__label" for="example-default-2">
        No
      </label>
    </div>
  </div>
</fieldset>
</div>

<div class="govuk-form-group">
  <fieldset class="govuk-fieldset" role="group" aria-describedby="dob-hint">
    <legend class="govuk-fieldset__legend">
      What is your date of birth?
    </legend>
    <div id="dob-hint" class="govuk-hint">
      For example, 31 3 1980
    </div>
    <div class="govuk-date-input" id="dob">
      <div class="govuk-date-input__item">
        <div class="govuk-form-group">
          <label class="govuk-label govuk-date-input__label" for="dob-day">
            Day
          </label>
          <input class="govuk-input govuk-date-input__input govuk-input--width-2" id="dob-day" name="day" type="text" inputmode="numeric">
        </div>
      </div>
      <div class="govuk-date-input__item">
        <div class="govuk-form-group">
          <label class="govuk-label govuk-date-input__label" for="dob-month">
            Month
          </label>
          <input class="govuk-input govuk-date-input__input govuk-input--width-2" id="dob-month" name="month" type="text" inputmode="numeric">
        </div>
      </div>
      <div class="govuk-date-input__item">
        <div class="govuk-form-group">
          <label class="govuk-label govuk-date-input__label" for="dob-year">
            Year
          </label>
          <input class="govuk-input govuk-date-input__input govuk-input--width-4" id="dob-year" name="year" type="text" inputmode="numeric">
        </div>
      </div>
    </div>
  </fieldset>
</div>

<hr class="govuk-section-break govuk-section-break--l govuk-section-break--visible">

<h2 class="govuk-heading-l">Summary list</h2>
<dl class="govuk-summary-list">
  <div class="govuk-summary-list__row">
    <dt class="govuk-summary-list__key">
      Name
    </dt>
    <dd class="govuk-summary-list__value">
      Firstname Lastname
    </dd>
  </div>
  <div class="govuk-summary-list__row">
    <dt class="govuk-summary-list__key">
      Date of birth
    </dt>
    <dd class="govuk-summary-list__value">
      13/08/1980
    </dd>
  </div>
  <div class="govuk-summary-list__row">
    <dt class="govuk-summary-list__key">
      Contact information
    </dt>
    <dd class="govuk-summary-list__value">
      <p class="govuk-body">
        email@email.com
      </p>
    </dd>
  </div>
</dl>

<hr class="govuk-section-break govuk-section-break--l govuk-section-break--visible">

<h2 class="govuk-heading-l">Table</h2>
<table class="govuk-table">
  <caption class="govuk-table__caption govuk-table__caption--m">Dates and amounts</caption>
  <thead class="govuk-table__head">
    <tr class="govuk-table__row">
      <th scope="col" class="govuk-table__header">Month</th>
      <th scope="col" class="govuk-table__header govuk-table__header--numeric">Income</th>
      <th scope="col" class="govuk-table__header govuk-table__header--numeric">Expenditure</th>
    </tr>
  </thead>
  <tbody class="govuk-table__body">
    <tr class="govuk-table__row">
      <th scope="row" class="govuk-table__header">January</th>
      <td class="govuk-table__cell govuk-table__cell--numeric">£85</td>
      <td class="govuk-table__cell govuk-table__cell--numeric">£95</td>
    </tr>
    <tr class="govuk-table__row">
      <th scope="row" class="govuk-table__header">February</th>
      <td class="govuk-table__cell govuk-table__cell--numeric">£75</td>
      <td class="govuk-table__cell govuk-table__cell--numeric">£55</td>
    </tr>
    <tr class="govuk-table__row">
      <th scope="row" class="govuk-table__header">March</th>
      <td class="govuk-table__cell govuk-table__cell--numeric">£165</td>
      <td class="govuk-table__cell govuk-table__cell--numeric">£125</td>
    </tr>
  </tbody>
</table>

<hr class="govuk-section-break govuk-section-break--l govuk-section-break--visible">

<h2 class="govuk-heading-l">Tabs</h2>
<div class="govuk-tabs" data-module="govuk-tabs">
  <h2 class="govuk-tabs__title">
    Contents
  </h2>
  <ul class="govuk-tabs__list">
    <li class="govuk-tabs__list-item govuk-tabs__list-item--selected">
      <a class="govuk-tabs__tab" href="#past-day">
        Past day
      </a>
    </li>
    <li class="govuk-tabs__list-item">
      <a class="govuk-tabs__tab" href="#past-week">
        Past week
      </a>
    </li>
    <li class="govuk-tabs__list-item">
      <a class="govuk-tabs__tab" href="#past-year">
        Past year
      </a>
    </li>
  </ul>
  <div class="govuk-tabs__panel" id="past-day">
    <h2 class="govuk-heading-l">Past day</h2>
    <p class="govuk-body">3 cases opened, 0 closed.</p>
  </div>
  <div class="govuk-tabs__panel govuk-tabs__panel--hidden" id="past-week">
    <h2 class="govuk-heading-l">Past week</h2>
    <p class="govuk-body">24 cases opened, 18 closed.</p>
  </div>
  <div class="govuk-tabs__panel govuk-tabs__panel--hidden" id="past-year">
    <p class="govuk-body">There is no data for this year yet, check back later</p>
  </div>
</div>

<hr class="govuk-section-break govuk-section-break--l govuk-section-break--visible">

<h2 class="govuk-heading-l">Accordion</h2>
<div class="govuk-accordion" data-module="govuk-accordion" id="default-example">
  <div class="govuk-accordion__section">
    <div class="govuk-accordion__section-header">
      <h2 class="govuk-accordion__section-heading">
        <span class="govuk-accordion__section-button" id="default-example-heading-1">
          Section A
        </span>
      </h2>
    </div>
    <div id="default-example-content-1" class="govuk-accordion__section-content">
      <p class="govuk-body">
        We need to know your nationality so we can work out which elections you’re entitled to vote in.
      </p>
    </div>
  </div>
  <div class="govuk-accordion__section">
    <div class="govuk-accordion__section-header">
      <h2 class="govuk-accordion__section-heading">
        <span class="govuk-accordion__section-button" id="default-example-heading-2">
          Section B
        </span>
      </h2>
    </div>
    <div id="default-example-content-2" class="govuk-accordion__section-content">
      <ul class="govuk-list govuk-list--bullet">
        <li>Example item 2</li>
      </ul>
    </div>
  </div>
</div>

<hr class="govuk-section-break govuk-section-break--l govuk-section-break--visible">

<h2 class="govuk-heading-l">Task list</h2>
<ul class="govuk-task-list">
  <li class="govuk-task-list__item govuk-task-list__item--with-link">
    <div class="govuk-task-list__name-and-hint">
      <a class="govuk-link govuk-task-list__link" href="#" aria-describedby="task-list-1-status">
        Company Directors
      </a>
    </div>
    <div class="govuk-task-list__status" id="task-list-1-status">
      Completed
    </div>
  </li>
  <li class="govuk-task-list__item govuk-task-list__item--with-link">
    <div class="govuk-task-list__name-and-hint">
      <a class="govuk-link govuk-task-list__link" href="#" aria-describedby="task-list-2-status">
        Registered company details
      </a>
    </div>
    <div class="govuk-task-list__status" id="task-list-2-status">
      <strong class="govuk-tag govuk-tag--blue">
        Incomplete
      </strong>
    </div>
  </li>
</ul>

<hr class="govuk-section-break govuk-section-break--l govuk-section-break--visible">

<h2 class="govuk-heading-l">Breadcrumbs</h2>
<nav class="govuk-breadcrumbs" aria-label="Breadcrumb">
  <ol class="govuk-breadcrumbs__list">
    <li class="govuk-breadcrumbs__list-item">
      <a class="govuk-breadcrumbs__link" href="#">Home</a>
    </li>
    <li class="govuk-breadcrumbs__list-item">
      <a class="govuk-breadcrumbs__link" href="#">Section</a>
    </li>
    <li class="govuk-breadcrumbs__list-item">
      <a class="govuk-breadcrumbs__link" href="#">Sub-section</a>
    </li>
  </ol>
</nav>

<hr class="govuk-section-break govuk-section-break--l govuk-section-break--visible">

<h2 class="govuk-heading-l">Pagination</h2>
<nav class="govuk-pagination" aria-label="Pagination">
  <div class="govuk-pagination__prev">
    <a class="govuk-link govuk-pagination__link" href="#" rel="prev">
      <svg class="govuk-pagination__icon govuk-pagination__icon--prev" xmlns="http://www.w3.org/2000/svg" height="13" width="15" aria-hidden="true" focusable="false" viewBox="0 0 15 13">
        <path d="m6.5938-0.0078125-6.7266 6.7266 6.7441 6.4062 1.377-1.449-4.1856-3.9768h12.896v-2h-12.984l4.2931-4.293-1.414-1.414z"></path>
      </svg>
      <span class="govuk-pagination__link-title">
        Previous<span class="govuk-visually-hidden"> page</span>
      </span>
    </a>
  </div>
  <ul class="govuk-pagination__list">
      <li class="govuk-pagination__item">
      <a class="govuk-link govuk-pagination__link" href="#" aria-label="Page 1">
        1
      </a>
    </li>
      <li class="govuk-pagination__item govuk-pagination__item--current">
      <a class="govuk-link govuk-pagination__link" href="#" aria-label="Page 2" aria-current="page">
        2
      </a>
    </li>
      <li class="govuk-pagination__item">
      <a class="govuk-link govuk-pagination__link" href="#" aria-label="Page 3">
        3
      </a>
    </li>
  </ul>
  <div class="govuk-pagination__next">
    <a class="govuk-link govuk-pagination__link" href="#" rel="next">
      <span class="govuk-pagination__link-title">
        Next<span class="govuk-visually-hidden"> page</span>
      </span>
      <svg class="govuk-pagination__icon govuk-pagination__icon--next" xmlns="http://www.w3.org/2000/svg" height="13" width="15" aria-hidden="true" focusable="false" viewBox="0 0 15 13">
        <path d="m8.107-0.0078125-1.4136 1.414 4.2926 4.293h-12.986v2h12.896l-4.1855 3.9766 1.377 1.4492 6.7441-6.4062-6.7246-6.7266z"></path>
      </svg>
    </a>
  </div>
</nav>

<hr class="govuk-section-break govuk-section-break--l govuk-section-break--visible">

<h2 class="govuk-heading-l">Phase banner</h2>
<div class="govuk-phase-banner govuk-width-container">
  <p class="govuk-phase-banner__content">
    <strong class="govuk-tag govuk-phase-banner__content__tag">
      Alpha
    </strong>
    <span class="govuk-phase-banner__text">
      This is a new service - your <a href="#" class="govuk-link">feedback</a> will help us to improve it.
    </span>
  </p>
</div>

<hr class="govuk-section-break govuk-section-break--l govuk-section-break--visible">
