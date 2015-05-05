---
layout: page-tile
type: page-styleguide-utilities
title: Layout
excerpt: These are single responsibility classes designed to help reduce duplication in our SCSS.
---

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Clearfix</h2>
    <p>Make an element expand to contain floated children. Uses pseudo-elements (micro clearfix).</p>
    <pre><code class=" language-sass" data-lang="scss">.u-cf</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">New Block Formatting Content</h2>
    <p>This affords some useful properties to the element. It won't wrap under floats. Will also contain any floated children. N.B. This will clip overflow. Use the alternative method below if this is problematic.</p>
    <pre><code class=" language-sass" data-lang="scss">.u-nbfc</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">New Block Formatting Content (Alternative)</h2>
    <p>Alternative method when overflow must not be clipped.</p>
    <pre><code class=" language-sass" data-lang="scss">.u-nbfcAlt</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Float Left</h2>
    <pre><code class=" language-sass" data-lang="scss">.u-floatLeft</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Float Right</h2>
    <pre><code class=" language-sass" data-lang="scss">.u-floatRight</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Float None</h2>
    <pre><code class=" language-sass" data-lang="scss">.u-floatNone</code></pre>
</div>


<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Full Height</h2>
    <pre><code class=" language-sass" data-lang="scss">.u-fullHeight</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Full Width</h2>
    <pre><code class=" language-sass" data-lang="scss">.u-fullWidth</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Center Align Content</h2>
    <pre><code class=" language-sass" data-lang="scss">.u-center</code></pre>
    <pre><code class=" language-sass" data-lang="scss">.u-centered</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Center Block Level Content</h2>
    <p>Uses <code>.u-textCenter</code>, <code>.u-fullWidth</code>, and <code>.u-center</code> to fully center a block of content.</p>
    <pre><code class=" language-sass" data-lang="scss">.u-centerBlock</code></pre>
</div>
