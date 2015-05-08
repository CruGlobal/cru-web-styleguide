---
layout: page
type: page-styleguide-components
title: Panels
---

While not always necessary, sometimes you need to put your DOM in a box. For those situations, try the panel component.

## Contents

* Will be replaced with the ToC, excluding the "Contents" header
{:toc}

## Basic example

By default, all the `.panel` does is apply some basic border and padding to contain some content.

{% example html %}
<div class="panel panel-default">
  <div class="panel-body">
    Basic panel example
  </div>
</div>
{% endexample %}


## Panel with headings

{% example html %}
<div class="panel panel-default">
  <div class="panel-heading">Panel heading without title</div>
  <div class="panel-body">
    Panel content
  </div>
</div>

<div class="panel panel-default">
  <div class="panel-heading">
    <h3 class="panel-title">Panel title</h3>
  </div>
  <div class="panel-body">
    Panel content
  </div>
</div>
{% endexample %}


## Panel with footer

Wrap buttons or secondary text in `.panel-footer`. Note that panel footers do not inherit colors and borders when using contextual variations as they are not meant to be in the foreground.

{% example html %}
<div class="panel panel-default">
  <div class="panel-body">
    Panel content
  </div>
  <div class="panel-footer">Panel footer</div>
</div>
{% endexample %}


## Panel with tables

Add any non-bordered `.table` within a panel for a seamless design. If there is a `.panel-body`, we add an extra border to the top of the table for separation.

{% example html %}
<div class="panel panel-default">
  <!-- Default panel contents -->
  <div class="panel-heading">Panel heading</div>
  <div class="panel-body">
    <p>Some default panel content here. Nulla vitae elit libero, a pharetra augue. Aenean lacinia bibendum nulla sed consectetur. Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis vestibulum. Nullam id dolor id nibh ultricies vehicula ut id elit.</p>
  </div>

  <!-- Table -->
  <table class="table">
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
</div>
{% endexample %}

If there is no panel body, the component moves from panel header to table without interruption.

{% example html %}
<div class="panel panel-default">
  <!-- Default panel contents -->
  <div class="panel-heading">Panel heading</div>

  <!-- Table -->
  <table class="table">
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
</div>
{% endexample %}

##

{% example html %}
{% endexample %}
