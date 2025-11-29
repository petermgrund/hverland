# GOV.UK Frontend Components Guide

This project now integrates the [GOV.UK Design System](https://design-system.service.gov.uk/) to provide consistent, accessible components for your Jekyll site.

## Setup

### Building Assets

Before running Jekyll, you need to build the GOV.UK Frontend assets:

```bash
npm install
npm run build
```

### Development Workflow

1. Build GOV.UK assets: `npm run build`
2. Run Jekyll: `bundle exec jekyll serve`

For live CSS recompilation during development:
```bash
npm run watch:css
```

## Available Components

All GOV.UK Design System components are now available. Here are the most commonly used ones:

### Buttons

```html
<button type="submit" class="govuk-button" data-module="govuk-button">
  Save and continue
</button>

<button type="submit" class="govuk-button govuk-button--secondary" data-module="govuk-button">
  Secondary Button
</button>

<button type="submit" class="govuk-button govuk-button--warning" data-module="govuk-button">
  Warning Button
</button>
```

### Typography

```html
<h1 class="govuk-heading-xl">Extra large heading</h1>
<h2 class="govuk-heading-l">Large heading</h2>
<h3 class="govuk-heading-m">Medium heading</h3>
<h4 class="govuk-heading-s">Small heading</h4>

<p class="govuk-body-l">Large body text</p>
<p class="govuk-body">Regular body text</p>
<p class="govuk-body-s">Small body text</p>
```

### Links

```html
<a href="#" class="govuk-link">Standard link</a>
<a href="#" class="govuk-link govuk-link--no-visited-state">Link with no visited state</a>
```

### Panels

```html
<div class="govuk-panel govuk-panel--confirmation">
  <h1 class="govuk-panel__title">Application complete</h1>
  <div class="govuk-panel__body">
    Your reference number<br><strong>HDJ2123F</strong>
  </div>
</div>
```

### Notification Banner

```html
<div class="govuk-notification-banner" role="region" aria-labelledby="govuk-notification-banner-title" data-module="govuk-notification-banner">
  <div class="govuk-notification-banner__header">
    <h2 class="govuk-notification-banner__title" id="govuk-notification-banner-title">
      Important
    </h2>
  </div>
  <div class="govuk-notification-banner__content">
    <p class="govuk-notification-banner__heading">
      You have 7 days left to send your application.
    </p>
  </div>
</div>
```

### Warning Text

```html
<div class="govuk-warning-text">
  <span class="govuk-warning-text__icon" aria-hidden="true">!</span>
  <strong class="govuk-warning-text__text">
    <span class="govuk-visually-hidden">Warning</span>
    You can be fined up to £5,000 if you don't register.
  </strong>
</div>
```

### Inset Text

```html
<div class="govuk-inset-text">
  It can take up to 8 weeks to register a lasting power of attorney if there are no mistakes in the application.
</div>
```

### Details (Accordion)

```html
<details class="govuk-details">
  <summary class="govuk-details__summary">
    <span class="govuk-details__summary-text">
      Help with nationality
    </span>
  </summary>
  <div class="govuk-details__text">
    We need to know your nationality so we can work out which elections you're entitled to vote in.
  </div>
</details>
```

### Summary List

```html
<dl class="govuk-summary-list">
  <div class="govuk-summary-list__row">
    <dt class="govuk-summary-list__key">
      Name
    </dt>
    <dd class="govuk-summary-list__value">
      Sarah Philips
    </dd>
    <dd class="govuk-summary-list__actions">
      <a class="govuk-link" href="#">
        Change<span class="govuk-visually-hidden"> name</span>
      </a>
    </dd>
  </div>
  <div class="govuk-summary-list__row">
    <dt class="govuk-summary-list__key">
      Date of birth
    </dt>
    <dd class="govuk-summary-list__value">
      5 January 1978
    </dd>
    <dd class="govuk-summary-list__actions">
      <a class="govuk-link" href="#">
        Change<span class="govuk-visually-hidden"> date of birth</span>
      </a>
    </dd>
  </div>
</dl>
```

### Table

```html
<table class="govuk-table">
  <caption class="govuk-table__caption govuk-table__caption--m">Dates and amounts</caption>
  <thead class="govuk-table__head">
    <tr class="govuk-table__row">
      <th scope="col" class="govuk-table__header">Date</th>
      <th scope="col" class="govuk-table__header">Amount</th>
    </tr>
  </thead>
  <tbody class="govuk-table__body">
    <tr class="govuk-table__row">
      <th scope="row" class="govuk-table__header">First 6 weeks</th>
      <td class="govuk-table__cell">£109.80 per week</td>
    </tr>
    <tr class="govuk-table__row">
      <th scope="row" class="govuk-table__header">Next 33 weeks</th>
      <td class="govuk-table__cell">£109.80 per week</td>
    </tr>
  </tbody>
</table>
```

### Tag

```html
<strong class="govuk-tag">Completed</strong>
<strong class="govuk-tag govuk-tag--blue">Active</strong>
<strong class="govuk-tag govuk-tag--green">New</strong>
<strong class="govuk-tag govuk-tag--red">Rejected</strong>
<strong class="govuk-tag govuk-tag--yellow">Pending</strong>
<strong class="govuk-tag govuk-tag--grey">Inactive</strong>
```

### Breadcrumbs

```html
<div class="govuk-breadcrumbs">
  <ol class="govuk-breadcrumbs__list">
    <li class="govuk-breadcrumbs__list-item">
      <a class="govuk-breadcrumbs__link" href="#">Home</a>
    </li>
    <li class="govuk-breadcrumbs__list-item">
      <a class="govuk-breadcrumbs__link" href="#">Section</a>
    </li>
    <li class="govuk-breadcrumbs__list-item">
      <a class="govuk-breadcrumbs__link">Subsection</a>
    </li>
  </ol>
</div>
```

### Phase Banner

```html
<div class="govuk-phase-banner">
  <p class="govuk-phase-banner__content">
    <strong class="govuk-tag govuk-phase-banner__content__tag">
      beta
    </strong>
    <span class="govuk-phase-banner__text">
      This is a new service – your <a class="govuk-link" href="#">feedback</a> will help us to improve it.
    </span>
  </p>
</div>
```

### Form Elements

#### Text Input
```html
<div class="govuk-form-group">
  <label class="govuk-label" for="event-name">
    Event name
  </label>
  <input class="govuk-input" id="event-name" name="event-name" type="text">
</div>
```

#### Textarea
```html
<div class="govuk-form-group">
  <label class="govuk-label" for="more-detail">
    Can you provide more detail?
  </label>
  <textarea class="govuk-textarea" id="more-detail" name="more-detail" rows="5"></textarea>
</div>
```

#### Radio Buttons
```html
<div class="govuk-form-group">
  <fieldset class="govuk-fieldset">
    <legend class="govuk-fieldset__legend govuk-fieldset__legend--l">
      <h1 class="govuk-fieldset__heading">
        Where do you live?
      </h1>
    </legend>
    <div class="govuk-radios" data-module="govuk-radios">
      <div class="govuk-radios__item">
        <input class="govuk-radios__input" id="where-do-you-live" name="where-do-you-live" type="radio" value="minnesota">
        <label class="govuk-label govuk-radios__label" for="where-do-you-live">
          Minnesota
        </label>
      </div>
      <div class="govuk-radios__item">
        <input class="govuk-radios__input" id="where-do-you-live-2" name="where-do-you-live" type="radio" value="elsewhere">
        <label class="govuk-label govuk-radios__label" for="where-do-you-live-2">
          Elsewhere
        </label>
      </div>
    </div>
  </fieldset>
</div>
```

#### Checkboxes
```html
<div class="govuk-form-group">
  <fieldset class="govuk-fieldset">
    <legend class="govuk-fieldset__legend govuk-fieldset__legend--l">
      <h1 class="govuk-fieldset__heading">
        Which types of waste do you transport?
      </h1>
    </legend>
    <div class="govuk-checkboxes" data-module="govuk-checkboxes">
      <div class="govuk-checkboxes__item">
        <input class="govuk-checkboxes__input" id="waste" name="waste" type="checkbox" value="animal">
        <label class="govuk-label govuk-checkboxes__label" for="waste">
          Waste from animal carcasses
        </label>
      </div>
      <div class="govuk-checkboxes__item">
        <input class="govuk-checkboxes__input" id="waste-2" name="waste" type="checkbox" value="mines">
        <label class="govuk-label govuk-checkboxes__label" for="waste-2">
          Waste from mines or quarries
        </label>
      </div>
    </div>
  </fieldset>
</div>
```

### Grid System

GOV.UK provides a responsive grid system:

```html
<div class="govuk-width-container">
  <div class="govuk-grid-row">
    <div class="govuk-grid-column-two-thirds">
      <h1 class="govuk-heading-xl">Two-thirds column</h1>
      <p class="govuk-body">Main content goes here.</p>
    </div>
    <div class="govuk-grid-column-one-third">
      <h2 class="govuk-heading-m">One-third column</h2>
      <p class="govuk-body">Sidebar content.</p>
    </div>
  </div>
</div>
```

Available column widths:
- `govuk-grid-column-full`
- `govuk-grid-column-one-half`
- `govuk-grid-column-one-third`
- `govuk-grid-column-two-thirds`
- `govuk-grid-column-one-quarter`
- `govuk-grid-column-three-quarters`

### Spacing Utilities

GOV.UK provides spacing utilities for consistent margins and padding:

```html
<!-- Margins -->
<div class="govuk-!-margin-bottom-0">No bottom margin</div>
<div class="govuk-!-margin-bottom-1">Small bottom margin</div>
<div class="govuk-!-margin-bottom-2">Medium bottom margin</div>
<div class="govuk-!-margin-bottom-4">Large bottom margin</div>
<div class="govuk-!-margin-bottom-8">Extra large bottom margin</div>

<!-- Top margins -->
<div class="govuk-!-margin-top-4">Top margin</div>

<!-- Padding -->
<div class="govuk-!-padding-4">Padding on all sides</div>
```

Available spacing values: 0, 1, 2, 3, 4, 5, 6, 7, 8, 9

### Typography Utilities

```html
<p class="govuk-!-font-size-80">Largest font size</p>
<p class="govuk-!-font-size-48">Large font size</p>
<p class="govuk-!-font-size-24">Medium font size</p>
<p class="govuk-!-font-size-19">Default font size</p>
<p class="govuk-!-font-size-16">Small font size</p>

<p class="govuk-!-font-weight-bold">Bold text</p>
<p class="govuk-!-font-weight-regular">Regular text</p>
```

## Layout Examples

### Two-column Layout with Sidebar

```html
<div class="govuk-width-container">
  <main class="govuk-main-wrapper">
    <div class="govuk-grid-row">
      <div class="govuk-grid-column-two-thirds">
        <h1 class="govuk-heading-xl">Page title</h1>
        <p class="govuk-body">Main content area</p>
      </div>
      <div class="govuk-grid-column-one-third">
        <aside class="govuk-!-margin-top-8">
          <h2 class="govuk-heading-m">Related content</h2>
          <nav>
            <ul class="govuk-list">
              <li><a class="govuk-link" href="#">Related link</a></li>
            </ul>
          </nav>
        </aside>
      </div>
    </div>
  </main>
</div>
```

### Publication Page

```html
<div class="govuk-width-container">
  <main class="govuk-main-wrapper" id="main-content">
    <div class="govuk-grid-row">
      <div class="govuk-grid-column-full">
        <span class="govuk-caption-l">Policy paper</span>
        <h1 class="govuk-heading-xl">Document title</h1>
      </div>
    </div>

    <div class="govuk-grid-row">
      <div class="govuk-grid-column-two-thirds">
        <div class="govuk-body">
          <p>Document content goes here.</p>
        </div>
      </div>

      <div class="govuk-grid-column-one-third">
        <aside>
          <h2 class="govuk-heading-s">Documents</h2>
          <a href="#" class="govuk-button govuk-button--secondary">Download PDF</a>
        </aside>
      </div>
    </div>
  </main>
</div>
```

## Color Palette

GOV.UK provides a consistent color palette accessible via CSS classes:

```html
<p class="govuk-!-colour-blue">Blue text</p>
```

Available colors: blue, green, yellow, red, grey-1, grey-2, grey-3, grey-4, black, white

## Resources

- [GOV.UK Design System](https://design-system.service.gov.uk/)
- [Component Examples](https://design-system.service.gov.uk/components/)
- [Style Guide](https://design-system.service.gov.uk/styles/)
- [Patterns](https://design-system.service.gov.uk/patterns/)

## Notes

- All components are accessible and follow WCAG 2.1 Level AA guidelines
- Components are responsive and work on all device sizes
- JavaScript is required for interactive components (accordion, character count, etc.)
- The `window.GOVUKFrontend.initAll()` in the default layout initializes all components
