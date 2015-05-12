---
layout: page-tile
type: page-styleguide-utilities
title: Utilities
excerpt: These are single responsibility classes designed to help reduce duplication in our SCSS.
---

<div class="panel  panel-default  p  markdown-body">
    <p class="mb-">We use <a href="https://github.com/thoughtbot/bourbon">Bourbon by Thoughtbot</a> as a mixin library. <a href="http://bourbon.io/docs/">Check it out</a> for a list of the available mixins</p>
    <p>We also use a few custom mixins for particular purposes. </p>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Center Block Content</h2>
    <p>You can also use the <code>u-centerBlock</code> utility class if you prefer to offload the work on the html. That is our preferred method but sometimes it is necessary to work in the scss.</p>
    <pre><code class=" language-sass" data-lang="scss">@mixin center-block()</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Clearfix</h2>
    <pre><code class=" language-sass" data-lang="scss">@mixin clearfix()</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">New Clearfix</h2>
    <pre><code class=" language-sass" data-lang="scss">@mixin pie-clearfix()</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Media Queries</h2>
    <p>Media query for easy breakpoint. Use pixel width with or without units and it will convert to em </p>
    <pre><code class=" language-sass" data-lang="scss">@mixin mq($point, $query1: min, $query2: width, $ie9: false)</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">REM Calculation</h2>
    <p>Can handle shorthand calculations</p>
    <pre><code class=" language-sass" data-lang="scss">@mixin rem-calc($property, $values)</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Spacings</h2>
    <p>Space elements by an amount based on your magic number. Pass in the property to be indented as a paramater</p>
    <pre><code class=" language-sass" data-lang="scss">@mixin spacing($property)</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Double Spacings</h2>
    <p>Space elements by an amount based on your magic number. Pass in the property to be indented as a paramater</p>
    <pre><code class=" language-sass" data-lang="scss">@mixin double-spacing($property)</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Half Spacings</h2>
    <p>Space elements by an amount based on your magic number. Pass in the property to be indented as a paramater</p>
    <pre><code class=" language-sass" data-lang="scss">@mixin half-spacing($property)</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Quarter Spacings</h2>
    <p>Space elements by an amount based on your magic number. Pass in the property to be indented as a paramater</p>
    <pre><code class=" language-sass" data-lang="scss">@mixin quarter-spacing($property)</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Eighth Spacings</h2>
    <p>Space elements by an amount based on your magic number. Pass in the property to be indented as a paramater</p>
    <pre><code class=" language-sass" data-lang="scss">@mixin eighth-spacing($property)</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Font Size</h2>
    <p>Quickly generate a font-size in rems, with a pixel fallback, based on the value we pass into the mixin and an optional line-height.</p>
    <pre><code class=" language-sass" data-lang="scss">@mixin font-size($font-size, $line-height: true) </code></pre>
</div>
