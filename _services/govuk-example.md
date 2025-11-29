---
layout: default
title: GOV.UK Components Example
description: A demonstration page showing various GOV.UK Design System components
---

<div class="govuk-width-container">
  <div class="govuk-phase-banner">
    <p class="govuk-phase-banner__content">
      <strong class="govuk-tag govuk-phase-banner__content__tag">
        beta
      </strong>
      <span class="govuk-phase-banner__text">
        This is a demonstration of GOV.UK components. Your <a class="govuk-link" href="#">feedback</a> will help us improve.
      </span>
    </p>
  </div>

  <main class="govuk-main-wrapper govuk-main-wrapper--auto-spacing" id="main-content" role="main">
    <div class="govuk-grid-row">
      <div class="govuk-grid-column-two-thirds">
        <h1 class="govuk-heading-xl">GOV.UK Components Demo</h1>
        <p class="govuk-body-l">
          This page demonstrates the integration of GOV.UK Design System components into the Minnesota.gov portal.
        </p>

        <h2 class="govuk-heading-l">Notification Banner</h2>
        <div class="govuk-notification-banner" role="region" aria-labelledby="govuk-notification-banner-title" data-module="govuk-notification-banner">
          <div class="govuk-notification-banner__header">
            <h2 class="govuk-notification-banner__title" id="govuk-notification-banner-title">
              Important
            </h2>
          </div>
          <div class="govuk-notification-banner__content">
            <p class="govuk-notification-banner__heading">
              This is an example notification banner to highlight important information.
            </p>
          </div>
        </div>

        <h2 class="govuk-heading-l">Buttons</h2>
        <button type="submit" class="govuk-button" data-module="govuk-button">
          Primary Button
        </button>

        <button type="submit" class="govuk-button govuk-button--secondary" data-module="govuk-button">
          Secondary Button
        </button>

        <button type="submit" class="govuk-button govuk-button--warning" data-module="govuk-button">
          Warning Button
        </button>

        <h2 class="govuk-heading-l govuk-!-margin-top-6">Warning Text</h2>
        <div class="govuk-warning-text">
          <span class="govuk-warning-text__icon" aria-hidden="true">!</span>
          <strong class="govuk-warning-text__text">
            <span class="govuk-visually-hidden">Warning</span>
            This is example warning text. It's used to warn users about important information.
          </strong>
        </div>

        <h2 class="govuk-heading-l">Inset Text</h2>
        <div class="govuk-inset-text">
          This is inset text. Use it to differentiate a block of text from the content that surrounds it, for example quotes or examples.
        </div>

        <h2 class="govuk-heading-l">Details (Accordion)</h2>
        <details class="govuk-details">
          <summary class="govuk-details__summary">
            <span class="govuk-details__summary-text">
              What is GOV.UK Design System?
            </span>
          </summary>
          <div class="govuk-details__text">
            The GOV.UK Design System provides styles, components and patterns to help government service teams create accessible, consistent user experiences. It's maintained by the Government Digital Service (GDS) in the UK.
          </div>
        </details>

        <h2 class="govuk-heading-l">Tags</h2>
        <p class="govuk-body">
          <strong class="govuk-tag">Completed</strong>
          <strong class="govuk-tag govuk-tag--blue">Active</strong>
          <strong class="govuk-tag govuk-tag--green">New</strong>
          <strong class="govuk-tag govuk-tag--red">Rejected</strong>
          <strong class="govuk-tag govuk-tag--yellow">Pending</strong>
          <strong class="govuk-tag govuk-tag--grey">Inactive</strong>
        </p>

        <h2 class="govuk-heading-l">Summary List</h2>
        <dl class="govuk-summary-list">
          <div class="govuk-summary-list__row">
            <dt class="govuk-summary-list__key">
              Component Library
            </dt>
            <dd class="govuk-summary-list__value">
              GOV.UK Design System
            </dd>
          </div>
          <div class="govuk-summary-list__row">
            <dt class="govuk-summary-list__key">
              Version
            </dt>
            <dd class="govuk-summary-list__value">
              5.13.0
            </dd>
          </div>
          <div class="govuk-summary-list__row">
            <dt class="govuk-summary-list__key">
              Status
            </dt>
            <dd class="govuk-summary-list__value">
              Active
            </dd>
          </div>
        </dl>

        <h2 class="govuk-heading-l">Table</h2>
        <table class="govuk-table">
          <caption class="govuk-table__caption govuk-table__caption--m">Component Features</caption>
          <thead class="govuk-table__head">
            <tr class="govuk-table__row">
              <th scope="col" class="govuk-table__header">Feature</th>
              <th scope="col" class="govuk-table__header">Available</th>
            </tr>
          </thead>
          <tbody class="govuk-table__body">
            <tr class="govuk-table__row">
              <th scope="row" class="govuk-table__header">Accessibility</th>
              <td class="govuk-table__cell">WCAG 2.1 Level AA</td>
            </tr>
            <tr class="govuk-table__row">
              <th scope="row" class="govuk-table__header">Responsive Design</th>
              <td class="govuk-table__cell">Yes</td>
            </tr>
            <tr class="govuk-table__row">
              <th scope="row" class="govuk-table__header">Browser Support</th>
              <td class="govuk-table__cell">Modern browsers + IE11</td>
            </tr>
          </tbody>
        </table>

      </div>

      <div class="govuk-grid-column-one-third">
        <aside class="govuk-!-padding-top-0">
          <h2 class="govuk-heading-m">Related Content</h2>
          <nav>
            <ul class="govuk-list govuk-list--spaced">
              <li>
                <a class="govuk-link" href="https://design-system.service.gov.uk/">GOV.UK Design System</a>
              </li>
              <li>
                <a class="govuk-link" href="https://design-system.service.gov.uk/components/">Component Library</a>
              </li>
              <li>
                <a class="govuk-link" href="https://design-system.service.gov.uk/styles/">Styles Guide</a>
              </li>
              <li>
                <a class="govuk-link" href="/GOVUK_COMPONENTS.html">Component Documentation</a>
              </li>
            </ul>
          </nav>

          <hr class="govuk-section-break govuk-section-break--m govuk-section-break--visible">

          <h3 class="govuk-heading-s">Quick Facts</h3>
          <div class="govuk-inset-text govuk-!-margin-top-0">
            All components are tested for accessibility and work across all modern browsers and assistive technologies.
          </div>
        </aside>
      </div>
    </div>
  </main>
</div>
