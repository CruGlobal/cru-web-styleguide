---
layout: page
type: page-styleguide-components
title: Buttons
---

## Contents

* Will be replaced with the ToC, excluding the "Contents" header
{:toc}

## Tags

Use the button classes on an `<a>`, `<button>`, or `<input>` element.

{% example html %}
  <a role="button" class="btn btn-subtle">Link</a>
  <button type="button" class="btn btn-subtle">Button</button>
  <input type="button" class="btn btn-subtle" value="Input"></input>
  <input type="submit" class="btn btn-subtle" value="Submit"></input>
{% endexample %}


## Options

Use any of the available button classes to quickly create a styled button.

{% example html %}
<!-- Our most used button -->
<button type="button" class="btn btn-subtle">Subtle</button>

<!-- Provides extra visual weight and identifies the primary action in a set of buttons -->
<button type="button" class="btn btn-primary">Primary</button>

<!-- Provides extra visual weight and identifies the primary action in a set of buttons -->
<button type="button" class="btn btn-secondary">Secondary</button>

<!-- Indicates a successful or positive action -->
<button type="button" class="btn btn-success">Success</button>

<!-- Contextual button for informational alert messages -->
<button type="button" class="btn btn-info">Info</button>

<!-- Indicates caution should be taken with this action -->
<button type="button" class="btn btn-warning">Warning</button>

<!-- Indicates a dangerous or potentially negative action -->
<button type="button" class="btn btn-danger">Danger</button>

<!-- Deemphasize a button by making it look like a link while maintaining button behavior -->
<button type="button" class="btn btn-link">Link</button>
{% endexample %}


## Sizes

Fancy larger or smaller buttons? Add `.btn-lg` or `.btn-sm`for additional sizes.
{% example html %}
<p>
  <button type="button" class="btn btn-primary btn-lg">Large button</button>
  <button type="button" class="btn btn-subtle btn-lg">Large button</button>
</p>
<p>
  <button type="button" class="btn btn-secondary">Default button</button>
  <button type="button" class="btn btn-subtle">Default button</button>
</p>
<p>
  <button type="button" class="btn btn-primary btn-sm">Small button</button>
  <button type="button" class="btn btn-subtle btn-sm">Small button</button>
</p>
{% endexample %}


## Block Level

Create block level buttons—those that span the full width of a parent— by adding `.btn-block`.

{% example html %}
<button type="button" class="btn btn-primary btn-lg btn-block">Block level button</button>
<button type="button" class="btn btn-subtle btn-lg btn-block">Block level button</button>
{% endexample %}
