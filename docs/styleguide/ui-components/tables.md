---
layout: page
type: page-styleguide-components
title: Tables
---

## Contents

* Will be replaced with the ToC, excluding the "Contents" header
{:toc}

## Basic Example

For basic styling—light padding and only horizontal dividers—add the base class `.table` to any `<table>`. It may seem super redundant, but given the widespread use of tables for other plugins like calendars and date pickers, we've opted to isolate our custom table styles.


{% example html %}
<table class="table">
      <caption>Optional table caption.</caption>
      <thead>
        <tr>
          <th>#</th>
          <th>First Name</th>
          <th>Last Name</th>
          <th>Username</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <th scope="row">1</th>
          <td>Jimmy</td>
          <td>Dempsey</td>
          <td>@thejamesdempsey</td>
        </tr>
        <tr>
          <th scope="row">2</th>
          <td>Matt</td>
          <td>Gasior</td>
          <td>@mattgasior</td>
        </tr>
        <tr>
          <th scope="row">3</th>
          <td>Jonathan</td>
          <td>Clark</td>
          <td>@jclarkcreative</td>
        </tr>
      </tbody>
    </table>
{% endexample %}


## Striped rows

Use `.table-striped` to add zebra-striping to any table row within the `<tbody>`.

<div class="docs-callout docs-callout-danger">
    <h4 id="cross-browser-compatibility">Cross-browser compatibility<a class="anchorjs-link" href="#cross-browser-compatibility"><span class="anchorjs-icon"></span></a></h4>
    <p>Striped tables are styled via the <code>:nth-child</code> CSS selector, which is not available in Internet Explorer 8.</p>
</div>


{% example html %}
<table class="table  table-striped">
  <thead>
    <tr>
      <th>#</th>
      <th>First Name</th>
      <th>Last Name</th>
      <th>Username</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">1</th>
      <td>Jimmy</td>
      <td>Dempsey</td>
      <td>@thejamesdempsey</td>
    </tr>
    <tr>
      <th scope="row">2</th>
      <td>Matt</td>
      <td>Gasior</td>
      <td>@mattgasior</td>
    </tr>
    <tr>
      <th scope="row">3</th>
      <td>Jonathan</td>
      <td>Clark</td>
      <td>@jclarkcreative</td>
    </tr>
  </tbody>
</table>
{% endexample %}

## Bordered table

Add `.table-bordered` for borders on all sides of the table and cells.

{% example html %}
<table class="table  table-bordered">
  <thead>
    <tr>
      <th>#</th>
      <th>First Name</th>
      <th>Last Name</th>
      <th>Username</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">1</th>
      <td>Jimmy</td>
      <td>Dempsey</td>
      <td>@thejamesdempsey</td>
    </tr>
    <tr>
      <th scope="row">2</th>
      <td>Matt</td>
      <td>Gasior</td>
      <td>@mattgasior</td>
    </tr>
    <tr>
      <th scope="row">3</th>
      <td>Jonathan</td>
      <td>Clark</td>
      <td>@jclarkcreative</td>
    </tr>
  </tbody>
</table>
{% endexample %}


## Hover rows

Add `.table-hover` to enable a hover state on table rows within a `<tbody>`.

{% example html%}
<table class="table  table-hover">
  <thead>
    <tr>
      <th>#</th>
      <th>First Name</th>
      <th>Last Name</th>
      <th>Username</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">1</th>
      <td>Jimmy</td>
      <td>Dempsey</td>
      <td>@thejamesdempsey</td>
    </tr>
    <tr>
      <th scope="row">2</th>
      <td>Matt</td>
      <td>Gasior</td>
      <td>@mattgasior</td>
    </tr>
    <tr>
      <th scope="row">3</th>
      <td>Jonathan</td>
      <td>Clark</td>
      <td>@jclarkcreative</td>
    </tr>
  </tbody>
</table>
{% endexample %}


## Condensed table

Add `.table-condensed` to make tables more compact by cutting cell padding in half.

{% example html%}
<table class="table  table-condensed">
  <thead>
    <tr>
      <th>#</th>
      <th>First Name</th>
      <th>Last Name</th>
      <th>Username</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">1</th>
      <td>Jimmy</td>
      <td>Dempsey</td>
      <td>@thejamesdempsey</td>
    </tr>
    <tr>
      <th scope="row">2</th>
      <td>Matt</td>
      <td>Gasior</td>
      <td>@mattgasior</td>
    </tr>
    <tr>
      <th scope="row">3</th>
      <td>Jonathan</td>
      <td>Clark</td>
      <td>@jclarkcreative</td>
    </tr>
  </tbody>
</table>
{% endexample %}


## Responsive tables

<div class="docs-callout docs-callout-warning">
    <h4 id="cross-browser-compatibility">Vertical clipping/truncation<span class="anchorjs-icon"></span></a></h4>
    <p>Responsive tables make use of `overflow-y: hidden`, which clips off any content that goes beyond the bottom or top edges of the table. In particular, this can clip off dropdown menus and other third-party widgets.</p>
</div>

<div class="docs-callout docs-callout-warning">
    <h4 id="cross-browser-compatibility">Firefox and fieldsets><span class="anchorjs-icon"></span></a></h4>
    <p>Firefox has some awkward fieldset styling involving `width` that interferes with the responsive table. This cannot be overriden without a Firefox-specific hack that we don't provide:</p>
<pre><code class="language-scss">
@-moz-document url-prefix() {
    fieldset { display: table-cell; }
}
</code>
</pre>
    For more information, read <a href="http://stackoverflow.com/questions/17408815/fieldset-resizes-wrong-appears-to-have-unremovable-min-width-min-content/17863685#17863685">this Stack Overflow answer</a>
</div>

{% example html%}
<div class="table-responsive">
      <table class="table">
        <thead>
          <tr>
            <th>#</th>
            <th>Table heading</th>
            <th>Table heading</th>
            <th>Table heading</th>
            <th>Table heading</th>
            <th>Table heading</th>
            <th>Table heading</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <th scope="row">1</th>
            <td>Table cell</td>
            <td>Table cell</td>
            <td>Table cell</td>
            <td>Table cell</td>
            <td>Table cell</td>
            <td>Table cell</td>
          </tr>
          <tr>
            <th scope="row">2</th>
            <td>Table cell</td>
            <td>Table cell</td>
            <td>Table cell</td>
            <td>Table cell</td>
            <td>Table cell</td>
            <td>Table cell</td>
          </tr>
          <tr>
            <th scope="row">3</th>
            <td>Table cell</td>
            <td>Table cell</td>
            <td>Table cell</td>
            <td>Table cell</td>
            <td>Table cell</td>
            <td>Table cell</td>
          </tr>
        </tbody>
      </table>
    </div>
{% endexample %}
