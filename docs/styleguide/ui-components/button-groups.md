---
layout: page
type: page-styleguide-components
title: Button Groups
excerpt: Group a series of buttons together on a single line with the button group.Add on optional JavaScript radio and checkbox style behavior with <a href="http://getbootstrap.com/javascript/#buttons">Bootstrap's buttons plugin</a>.
---

## Contents

* Will be replaced with the ToC, excluding the "Contents" header
{:toc}

## Basic

Wrap a series of buttons with `.btn` in `.btn-group`.

{% example html %}
<div class="btn-group" role="group" aria-label="...">
  <button type="button" class="btn btn-subtle">Left</button>
  <button type="button" class="btn btn-subtle">Middle</button>
  <button type="button" class="btn btn-subtle">Right</button>
</div>
{% endexample %}

## Toolbar

Combine sets of `<div class="btn-group">` into a `<div class="btn-toolbar">` for more complex components.

{% example html %}
<div class="btn-toolbar" role="toolbar" aria-label="...">
  <div class="btn-group" role="group" aria-label="...">
    <button type="button" class="btn btn-subtle">1</button>
    <button type="button" class="btn btn-subtle">2</button>
  </div>
  <div class="btn-group" role="group" aria-label="...">
    <button type="button" class="btn btn-subtle">3</button>
    <button type="button" class="btn btn-subtle">4</button>

  </div>
  <div class="btn-group" role="group" aria-label="...">
  <button type="button" class="btn btn-subtle">5</button>
  </div>
</div>
{% endexample %}


## Sizing

Instead of applying button sizing classes to every button in a group, just add `.btn-group-*` to each `.btn-group`, including when nesting multiple groups.

{% example html %}
<div class="btn-group btn-group-lg" role="group" aria-label="...">
    <button type="button" class="btn btn-subtle">Left</button>
    <button type="button" class="btn btn-subtle">Middle</button>
    <button type="button" class="btn btn-subtle">Right</button>
</div>
<div class="btn-group" role="group" aria-label="...">
    <button type="button" class="btn btn-subtle">Left</button>
    <button type="button" class="btn btn-subtle">Middle</button>
    <button type="button" class="btn btn-subtle">Right</button>
</div>
<div class="btn-group btn-group-sm" role="group" aria-label="...">
    <button type="button" class="btn btn-subtle">Left</button>
    <button type="button" class="btn btn-subtle">Middle</button>
    <button type="button" class="btn btn-subtle">Right</button>
</div>
{% endexample %}


## Nesting

Place a `.btn-group` within another `.btn-group` when you want dropdown menus mixed with a series of buttons.

{% example html %}
<div class="btn-group" role="group" aria-label="...">
  <button type="button" class="btn btn-subtle">1</button>
  <button type="button" class="btn btn-subtle">2</button>

  <div class="btn-group" role="group">
    <button type="button" class="btn btn-subtle dropdown-toggle" data-toggle="dropdown" aria-expanded="false">
      Dropdown
      <span class="caret"></span>
    </button>
    <ul class="dropdown-menu" role="menu">
      <li><a href="#">Dropdown link</a></li>
      <li><a href="#">Dropdown link</a></li>
    </ul>
  </div>
</div>
{% endexample %}



## Vertical Variation

Make a set of buttons appear vertically stacked rather than horizontally. Split button dropdowns are not supported here.

{% example html %}
<div class="btn-group-vertical" role="group" aria-label="Vertical button group">
      <button type="button" class="btn btn-subtle">Button</button>
      <button type="button" class="btn btn-subtle">Button</button>
      <div class="btn-group" role="group">
        <button id="btnGroupVerticalDrop1" type="button" class="btn btn-subtle dropdown-toggle" data-toggle="dropdown" aria-expanded="false">
          Dropdown
          <span class="caret"></span>
        </button>
        <ul class="dropdown-menu" role="menu" aria-labelledby="btnGroupVerticalDrop1">
          <li><a href="#">Dropdown link</a></li>
          <li><a href="#">Dropdown link</a></li>
        </ul>
      </div>
      <button type="button" class="btn btn-subtle">Button</button>
      <button type="button" class="btn btn-subtle">Button</button>
      <div class="btn-group" role="group">
        <button id="btnGroupVerticalDrop2" type="button" class="btn btn-subtle dropdown-toggle" data-toggle="dropdown" aria-expanded="false">
          Dropdown
          <span class="caret"></span>
        </button>
        <ul class="dropdown-menu" role="menu" aria-labelledby="btnGroupVerticalDrop2">
          <li><a href="#">Dropdown link</a></li>
          <li><a href="#">Dropdown link</a></li>
        </ul>
      </div>
      <div class="btn-group" role="group">
        <button id="btnGroupVerticalDrop3" type="button" class="btn btn-subtle dropdown-toggle" data-toggle="dropdown" aria-expanded="false">
          Dropdown
          <span class="caret"></span>
        </button>
        <ul class="dropdown-menu" role="menu" aria-labelledby="btnGroupVerticalDrop3">
          <li><a href="#">Dropdown link</a></li>
          <li><a href="#">Dropdown link</a></li>
        </ul>
      </div>
      <div class="btn-group" role="group">
        <button id="btnGroupVerticalDrop4" type="button" class="btn btn-subtle dropdown-toggle" data-toggle="dropdown" aria-expanded="false">
          Dropdown
          <span class="caret"></span>
        </button>
        <ul class="dropdown-menu" role="menu" aria-labelledby="btnGroupVerticalDrop4">
          <li><a href="#">Dropdown link</a></li>
          <li><a href="#">Dropdown link</a></li>
        </ul>
      </div>
    </div>
{% endexample %}
