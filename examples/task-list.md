---
layout: default
title: Task list
permalink: /examples/task-list/
---

<div class="govuk-grid-row">
  <div class="govuk-grid-column-two-thirds">

    <h1 class="govuk-heading-xl">
      {{ site.title }}
    </h1>

    <h2 class="govuk-heading-s govuk-!-margin-bottom-2">Application incomplete</h2>
    <p class="govuk-body govuk-!-margin-bottom-7">You have completed 3 of 8 sections.</p>

    <h2 class="govuk-heading-m">1. Check before you start</h2>
    <ul class="govuk-task-list">
      <li class="govuk-task-list__item govuk-task-list__item--with-link">
        <div class="govuk-task-list__name-and-hint">
          <a class="govuk-link govuk-task-list__link" href="#" aria-describedby="eligibility-status">
            Check eligibility
          </a>
        </div>
        <div class="govuk-task-list__status" id="eligibility-status">
          Completed
        </div>
      </li>
      <li class="govuk-task-list__item govuk-task-list__item--with-link">
        <div class="govuk-task-list__name-and-hint">
          <a class="govuk-link govuk-task-list__link" href="#" aria-describedby="read-declaration-status">
            Read declaration
          </a>
        </div>
        <div class="govuk-task-list__status" id="read-declaration-status">
          Completed
        </div>
      </li>
    </ul>

    <h2 class="govuk-heading-m">2. Prepare application</h2>
    <ul class="govuk-task-list">
      <li class="govuk-task-list__item govuk-task-list__item--with-link">
        <div class="govuk-task-list__name-and-hint">
          <a class="govuk-link govuk-task-list__link" href="#" aria-describedby="company-information-status">
            Company information
          </a>
        </div>
        <div class="govuk-task-list__status" id="company-information-status">
          Completed
        </div>
      </li>
      <li class="govuk-task-list__item govuk-task-list__item--with-link">
        <div class="govuk-task-list__name-and-hint">
          <a class="govuk-link govuk-task-list__link" href="#" aria-describedby="contact-details-status">
            Your contact details
          </a>
        </div>
        <div class="govuk-task-list__status" id="contact-details-status">
          <strong class="govuk-tag govuk-tag--blue">In progress</strong>
        </div>
      </li>
      <li class="govuk-task-list__item govuk-task-list__item--with-link">
        <div class="govuk-task-list__name-and-hint">
          <a class="govuk-link govuk-task-list__link" href="#" aria-describedby="list-convictions-status">
            List convictions
          </a>
        </div>
        <div class="govuk-task-list__status" id="list-convictions-status">
          <strong class="govuk-tag govuk-tag--grey">Not started</strong>
        </div>
      </li>
      <li class="govuk-task-list__item">
        <div class="govuk-task-list__name-and-hint">
          Provide financial evidence
        </div>
        <div class="govuk-task-list__status" id="financial-evidence-status">
          <strong class="govuk-tag govuk-tag--grey">Cannot start yet</strong>
        </div>
      </li>
      <li class="govuk-task-list__item">
        <div class="govuk-task-list__name-and-hint">
          Give medical information
        </div>
        <div class="govuk-task-list__status" id="medical-information-status">
          <strong class="govuk-tag govuk-tag--grey">Cannot start yet</strong>
        </div>
      </li>
    </ul>

    <h2 class="govuk-heading-m">3. Apply</h2>
    <ul class="govuk-task-list">
      <li class="govuk-task-list__item">
        <div class="govuk-task-list__name-and-hint">
          Submit and pay
        </div>
        <div class="govuk-task-list__status" id="submit-pay-status">
          <strong class="govuk-tag govuk-tag--grey">Cannot start yet</strong>
        </div>
      </li>
    </ul>

  </div>
</div>
