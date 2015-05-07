---
layout: page
type: page-styleguide-components
title: Navs
---

All of the navs available have shared markup, starting with the base `.nav` class, as well as shared states. Swap modifier classes to switch between each style.

If you are using navs to provide a navigation bar, be sure to add a `role="navigation"` to the most logical parent container of the `<ul>`, or wrap a `<nav>` element around the whole navigation. Do not add the role to the `<ul>` itself, as this would prevent it from being announced as an actual list by assistive technologies.

## Contents

* Will be replaced with the ToC, excluding the "Contents" header
{:toc}

## Tabs
Note the `.nav-tabs` class requires the `.nav` base class.

{% example html %}
<ul class="nav  nav-tabs">
  <li role="presentation" class="active"><a href="#">Home</a></li>
  <li role="presentation"><a href="#">Profile</a></li>
  <li role="presentation"><a href="#">Messages</a></li>
</ul>
{% endexample %}


## Pills
Take that same HTML, but use `.nav-pills` instead:

{% example html %}
<ul class="nav  nav-pills">
  <li role="presentation" class="active"><a href="#">Home</a></li>
  <li role="presentation"><a href="#">Profile</a></li>
  <li role="presentation"><a href="#">Messages</a></li>
</ul>
{% endexample %}

Pills are also vertically stackable. Just add `.nav-stacked`.

{% example html %}
<ul class="nav  nav-pills  nav-stacked">
  <li role="presentation" class="active"><a href="#">Home</a></li>
  <li role="presentation"><a href="#">Profile</a></li>
  <li role="presentation"><a href="#">Messages</a></li>
</ul>
{% endexample %}

## Justified

Easily make tabs or pills equal widths of their parent at screens wider than 768px with `.nav-justified`. On smaller screens, the nav links are stacked.

Justified navbar nav links are currently not supported.

{% example html %}
<ul class="nav  nav-pills  nav-justified">
  <li role="presentation" class="active"><a href="#">Home</a></li>
  <li role="presentation"><a href="#">Profile</a></li>
  <li role="presentation"><a href="#">Messages</a></li>
</ul>
{% endexample %}

{% example html %}
<ul class="nav  nav-tabs  nav-justified">
  <li role="presentation" class="active"><a href="#">Home</a></li>
  <li role="presentation"><a href="#">Profile</a></li>
  <li role="presentation"><a href="#">Messages</a></li>
</ul>
{% endexample %}


## Disabled Links

For any nav component (tabs or pills), add `.disabled` for gray links and no hover effects.

{% example html %}
<ul class="nav  nav-pills">
    <li role="presentation"><a href="#">Clickable link</a></li>
    <li role="presentation"><a href="#">Clickable link</a></li>
    <li role="presentation" class="disabled"><a href="#">Disabled link</a></li>
</ul>
{% endexample %}


## Using Dropdowns

Add dropdown menus with a little extra HTML and the <a href="http://getbootstrap.com/javascript/#dropdowns">dropdowns JavaScript plugin</a>.


### Tabs with dropdowns

{% example html %}
<ul class="nav nav-tabs">
  <li role="presentation" class="active"><a href="#">Home</a></li>
  <li role="presentation"><a href="#">Help</a></li>
  <li role="presentation" class="dropdown">
    <a class="dropdown-toggle" data-toggle="dropdown" href="#" role="button" aria-expanded="false">
      Dropdown <span class="caret"></span>
    </a>
    <ul class="dropdown-menu" role="menu">
      <li><a href="#">Action</a></li>
      <li><a href="#">Another action</a></li>
      <li><a href="#">Something else here</a></li>
      <li class="divider"></li>
      <li><a href="#">Separated link</a></li>
    </ul>
  </li>
</ul>
{% endexample %}


### Pills with dropdowns

{% example html %}
<ul class="nav nav-pills">
  <li role="presentation" class="active"><a href="#">Home</a></li>
  <li role="presentation"><a href="#">Help</a></li>
  <li role="presentation" class="dropdown">
    <a class="dropdown-toggle" data-toggle="dropdown" href="#" role="button" aria-expanded="false">
      Dropdown <span class="caret"></span>
    </a>
    <ul class="dropdown-menu" role="menu">
      <li><a href="#">Action</a></li>
      <li><a href="#">Another action</a></li>
      <li><a href="#">Something else here</a></li>
      <li class="divider"></li>
      <li><a href="#">Separated link</a></li>
    </ul>
  </li>
</ul>
{% endexample %}
