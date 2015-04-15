---
layout: page
title: Layout
---

Bootstrap includes a responsive, mobile first fluid grid system that appropriately scales up to 12 columns as the device or viewport size increases. It includes predefined classes for easy layout options, as well as powerful mixins for generating more semantic layouts.

You can reference their documentation on their [Grid](http://getbootstrap.com/css/#grid).

## Contents

* Will be replaced with the ToC, excluding the "Contents" header
{:toc}

## Container

Center your page's contents with a `.container`.

{% highlight html %}
<div class="container">
  <!-- contents here -->
</div>
{% endhighlight %}

The container applies `width: 980px;` and uses horizontal `margin`s to center it.

## Grid

The grid is pretty standard—you create rows with `.columns` and individual columns with a column class and fraction class. Here's how it works:

- Add a `.container` to encapsulate everything and provide ample horizontal gutter space.
- Create your outer row to clear the floated columns with `<div class="columns">`.
- Add your columns with individual `<div class="column">`s.
- Add your fractional width classes to set the width of the columns (e.g., `.one-fourth`).

In practice, your columns will look like the example below.

{% example html %}
<div class="container">
  <div class="columns">
    <div class="one-fifth column">
      .one-fifth
    </div>
    <div class="four-fifths column">
      .four-fifths
    </div>
  </div>

  <div class="columns">
    <div class="one-fourth column">
      .one-fourth
    </div>
    <div class="three-fourths column">
      .three-fourths
    </div>
  </div>

  <div class="columns">
    <div class="one-third column">
      .one-third
    </div>
    <div class="two-thirds column">
      .two-thirds
    </div>
  </div>

  <div class="columns">
    <div class="one-half column">
      .one-half
    </div>
    <div class="one-half column">
      .one-half
    </div>
  </div>
</div>
{% endexample %}
