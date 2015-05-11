---
layout: page-tile
type: page-styleguide-utilities
title: Spacing
excerpt: These are single responsibility classes designed to help reduce duplication in our SCSS.
---

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Usage</h2>

    <p>The spacings classes are all based off a set margin and padding. This allows us to set a uniform scale. In the case of cru.org, we base this off of a uniform line height which controls many other things. </p>
<pre><code class=" language-sass" data-lang="scss">$base-margin:  $base-line-height !default;
$base-padding: $base-line-height !default;
</code></pre>


    <p>In order to use the spacing classes you must activate them by changing the variables to true. By default you will see:</p>
<pre><code class=" language-sass" data-lang="scss">$enable-margins:        false !default;
$enable-margins--tiny:  false !default;
$enable-margins--small: false !default;
$enable-margins--large: false !default;
$enable-margins--huge:  false !default;
$enable-margins--none:  false !default;

$enable-paddings:        false !default;
$enable-paddings--tiny:  false !default;
$enable-paddings--small: false !default;
$enable-paddings--large: false !default;
$enable-paddings--huge:  false !default;
$enable-paddings--none:  false !default;
</code></pre>

    <p>Do not override these variables directly. Set the ones you need to true in your projects main `.scss` file or in a variables specific file.</p>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Margins</h2>
<pre><code class=" language-sass" data-lang="scss">.m  { margin:        $base-margin !important; }
.mt { margin-top:    $base-margin !important; }
.mr { margin-right:  $base-margin !important; }
.mb { margin-bottom: $base-margin !important; }
.ml { margin-left:   $base-margin !important; }
.me { margin-top:    $base-margin !important; margin-bottom: $base-margin !important; }
.ms { margin-right:  $base-margin !important; margin-left:   $base-margin !important; }
</code></pre>
</div>


<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Margins Tiny</h2>
<pre><code class=" language-sass" data-lang="scss">.m--  { margin:        quarter($base-margin) !important; }
.mt-- { margin-top:    quarter($base-margin) !important; }
.mr-- { margin-right:  quarter($base-margin) !important; }
.mb-- { margin-bottom: quarter($base-margin) !important; }
.ml-- { margin-left:   quarter($base-margin) !important; }
.ms-- { margin-top:    quarter($base-margin) !important; margin-bottom: quarter($base-margin) !important; }
.me-- { margin-right:  quarter($base-margin) !important; margin-left:   quarter($base-margin) !important; }
</code></pre>
</div>


<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Margins Small</h2>
<pre><code class=" language-sass" data-lang="scss">.m-  { margin:        half($base-margin) !important; }
.mt- { margin-top:    half($base-margin) !important; }
.mr- { margin-right:  half($base-margin) !important; }
.mb- { margin-bottom: half($base-margin) !important; }
.ml- { margin-left:   half($base-margin) !important; }
.me- { margin-top:    half($base-margin) !important; margin-bottom: half($base-margin) !important; }
.ms- { margin-right:  half($base-margin) !important; margin-left:   half($base-margin) !important; }
</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Margins Large</h2>
<pre><code class=" language-sass" data-lang="scss">.m_x  { margin:        double($base-margin) !important;  }
.mt_x { margin-top:    double($base-margin) !important;  }
.mr_x { margin-right:  double($base-margin) !important;  }
.mb_x { margin-bottom: double($base-margin) !important;  }
.ml_x { margin-left:   double($base-margin) !important;  }
.me_x { margin-top:    double($base-margin) !important; margin-bottom:  double($base-margin) !important; }
.ms_x { margin-right:  double($base-margin) !important; margin-left:    double($base-margin) !important; }
</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Margins Huge</h2>
<pre><code class=" language-sass" data-lang="scss">.m_xx  { margin:        quadruple($base-margin) !important;  }
.mt_xx { margin-top:    quadruple($base-margin) !important;  }
.mr_xx { margin-right:  quadruple($base-margin) !important;  }
.mb_xx { margin-bottom: quadruple($base-margin) !important;  }
.ml_xx { margin-left:   quadruple($base-margin) !important;  }
.ms_xx { margin-top:    quadruple($base-margin) !important; margin-bottom: quadruple($base-margin) !important; }
.me_xx { margin-right:  quadruple($base-margin) !important; margin-left:   quadruple($base-margin) !important; }
</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Margins None</h2>
<pre><code class=" language-sass" data-lang="scss">.m0  { margin:        0 !important; }
.mt0 { margin-top:    0 !important; }
.mr0 { margin-right:  0 !important; }
.mb0 { margin-bottom: 0 !important; }
.ml0 { margin-left:   0 !important; }
.me0 { margin-top:    0 !important; margin-bottom: 0 !important; }
.ms0 { margin-right:  0 !important; margin-left:   0 !important; }
</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Paddings</h2>
<pre><code class=" language-sass" data-lang="scss">.p  { padding:        $base-padding !important; }
.pt { padding-top:    $base-padding !important; }
.pr { padding-right:  $base-padding !important; }
.pb { padding-bottom: $base-padding !important; }
.pl { padding-left:   $base-padding !important; }
.pe { padding-top:    $base-padding !important; padding-bottom: $base-padding !important; }
.ps { padding-right:  $base-padding !important; padding-left:   $base-padding !important; }
</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Paddings Tiny</h2>
<pre><code class=" language-sass" data-lang="scss">.p--  { padding:        quarter($base-padding) !important; }
.pt-- { padding-top:    quarter($base-padding) !important; }
.pr-- { padding-right:  quarter($base-padding) !important; }
.pb-- { padding-bottom: quarter($base-padding) !important; }
.pl-- { padding-left:   quarter($base-padding) !important; }
.pe-- { padding-top:    quarter($base-padding) !important; padding-bottom: quarter($base-padding) !important; }
.ps-- { padding-right:  quarter($base-padding) !important; padding-left:   quarter($base-padding) !important; }
</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Paddings Small</h2>
<pre><code class=" language-sass" data-lang="scss">.p-  { padding:        half($base-padding) !important; }
.pt- { padding-top:    half($base-padding) !important; }
.pr- { padding-right:  half($base-padding) !important; }
.pb- { padding-bottom: half($base-padding) !important; }
.pl- { padding-left:   half($base-padding) !important; }
.pe- { padding-top:    half($base-padding) !important; padding-bottom: half($base-padding) !important; }
.ps- { padding-right:  half($base-padding) !important; padding-left:   half($base-padding) !important; }

</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Paddings Large</h2>
<pre><code class=" language-sass" data-lang="scss">.p_x  { padding:        double($base-padding) !important; }
.pt_x { padding-top:    double($base-padding) !important; }
.pr_x { padding-right:  double($base-padding) !important; }
.pb_x { padding-bottom: double($base-padding) !important; }
.pl_x { padding-left:   double($base-padding) !important; }
.pe_x { padding-top:    double($base-padding) !important; padding-bottom: double($base-padding) !important; }
.ps_x { padding-right:  double($base-padding) !important; padding-left:   double($base-padding) !important; }
</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Paddings Huge</h2>
<pre><code class=" language-sass" data-lang="scss">.p_xx  { padding:        quadruple($base-padding) !important; }
.pt_xx { padding-top:    quadruple($base-padding) !important; }
.pr_xx { padding-right:  quadruple($base-padding) !important; }
.pb_xx { padding-bottom: quadruple($base-padding) !important; }
.pl_xx { padding-left:   quadruple($base-padding) !important; }
.pe_xx { padding-top:    quadruple($base-padding) !important; padding-bottom: quadruple($base-padding) !important; }
.ps_xx { padding-right:  quadruple($base-padding) !important; padding-left:   quadruple($base-padding) !important; }
</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Paddings None</h2>
<pre><code class=" language-sass" data-lang="scss">.p0  { padding:        0 !important; }
.pt0 { padding-top:    0 !important; }
.pr0 { padding-right:  0 !important; }
.pb0 { padding-bottom: 0 !important; }
.pl0 { padding-left:   0 !important; }
.pe0 { padding-top:    0 !important; padding-bottom: 0 !important; }
.ps0 { padding-right:  0 !important; padding-left:   0 !important; }
</code></pre>
</div>
