---
layout: page-tile
type: page-styleguide-utilities
title: Generic
excerpt: These are single responsibility classes designed to help reduce duplication in our SCSS.
---

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Align Text Left</h2>
    <pre><code class=" language-sass" data-lang="scss">%u-textLeft</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Align Text Center</h2>
    <pre><code class=" language-sass" data-lang="scss">%u-textCenter</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Align Text Right</h2>
    <pre><code class=" language-sass" data-lang="scss">%u-textRight</code></pre>
</div>


<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Vertical Align Baseline</h2>
    <pre><code class=" language-sass" data-lang="scss">%u-alignBaseline</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Vertical Align Top</h2>
    <pre><code class=" language-sass" data-lang="scss">%u-alignTop</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Vertical Align Middle</h2>
    <pre><code class=" language-sass" data-lang="scss">%u-alignMiddle</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Vertical Align Bottom</h2>
    <pre><code class=" language-sass" data-lang="scss">%u-alignBottom</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Display Block</h2>
    <pre><code class=" language-sass" data-lang="scss">%u-block</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Display Inline</h2>
    <pre><code class=" language-sass" data-lang="scss">%u-inline</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Display Inline Block</h2>
    <pre><code class=" language-sass" data-lang="scss">%u-inlineBlock</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Display None</h2>
    <p>Items should be set to <code>display: none;</code> with caution. This removes content entirely and should only be used if the content is being presented somewhere else or is not needed for the user. <code>%u-hiddenVisually</code> is preferred</p>
    <pre><code class=" language-sass" data-lang="scss">%u-hidden</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Visually Hidden</h2>
    <p>Completely remove from the flow but leave available to screen readers.</p>
    <pre><code class=" language-sass" data-lang="scss">%u-hiddenVisually</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Display Table</h2>
    <pre><code class=" language-sass" data-lang="scss">%u-table</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Display Table Cell</h2>
    <pre><code class=" language-sass" data-lang="scss">%u-tableCell</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Display Table Row</h2>
    <pre><code class=" language-sass" data-lang="scss">%u-tableRow</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Clearfix</h2>
    <p>Make an element expand to contain floated children. Uses pseudo-elements (micro clearfix).</p>
    <pre><code class=" language-sass" data-lang="scss">%u-cf</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">New Block Formatting Content</h2>
    <p>This affords some useful properties to the element. It won't wrap under floats. Will also contain any floated children. N.B. This will clip overflow. Use the alternative method below if this is problematic.</p>
    <pre><code class=" language-sass" data-lang="scss">%u-nbfc</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">New Block Formatting Content (Alternative)</h2>
    <p>Alternative method when overflow must not be clipped.</p>
    <pre><code class=" language-sass" data-lang="scss">%u-nbfcAlt</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Float Left</h2>
    <pre><code class=" language-sass" data-lang="scss">%u-floatLeft</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Float Right</h2>
    <pre><code class=" language-sass" data-lang="scss">%u-floatRight</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Float None</h2>
    <pre><code class=" language-sass" data-lang="scss">%u-floatNone</code></pre>
</div>


<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Full Height</h2>
    <pre><code class=" language-sass" data-lang="scss">%u-fullHeight</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Full Width</h2>
    <pre><code class=" language-sass" data-lang="scss">%u-fullWidth</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Center Align Content</h2>
    <pre><code class=" language-sass" data-lang="scss">%u-center</code></pre>
    <pre><code class=" language-sass" data-lang="scss">%u-centered</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Center Block Level Content</h2>
    <p>Uses <code>%u-textCenter</code>, <code>%u-fullWidth</code>, and <code>%u-center</code> to fully center a block of content.</p>
    <pre><code class=" language-sass" data-lang="scss">%u-centerBlock</code></pre>
</div>


<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Link Clean</h2>
    <p>A link without any text-decoration at all.</p>
    <pre><code class=" language-sass" data-lang="scss">%u-linkClean</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Link Block</h2>
    <p>Combination of traits commonly used in vertical navigation lists.</p>
    <pre><code class=" language-sass" data-lang="scss">%u-linkBlock</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Position Absolute</h2>
    <pre><code class=" language-sass" data-lang="scss">%u-posAbsolute</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Position Relative</h2>
    <pre><code class=" language-sass" data-lang="scss">%u-posRelative</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Position Static</h2>
    <pre><code class=" language-sass" data-lang="scss">%u-posStatic</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Position Fixed</h2>
    <pre><code class=" language-sass" data-lang="scss">%u-posFixed</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Position Absolute Center</h2>
    <p>Pins to all corners by default. But when a width and/or height are provided, the element will be centered in its nearest relatively-positioned ancestor.</p>
    <pre><code class=" language-sass" data-lang="scss">%u-posAbsoluteCenter</code></pre>
</div>



<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Margins</h2>
<pre><code class=" language-sass" data-lang="scss">%m  { margin:        $base-margin !important; }
%mt { margin-top:    $base-margin !important; }
%mr { margin-right:  $base-margin !important; }
%mb { margin-bottom: $base-margin !important; }
%ml { margin-left:   $base-margin !important; }
%me { margin-top:    $base-margin !important; margin-bottom: $base-margin !important; }
%ms { margin-right:  $base-margin !important; margin-left:   $base-margin !important; }
</code></pre>
</div>


<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Margins Tiny</h2>
<pre><code class=" language-sass" data-lang="scss">%m--  { margin:        quarter($base-margin) !important; }
%mt-- { margin-top:    quarter($base-margin) !important; }
%mr-- { margin-right:  quarter($base-margin) !important; }
%mb-- { margin-bottom: quarter($base-margin) !important; }
%ml-- { margin-left:   quarter($base-margin) !important; }
%ms-- { margin-top:    quarter($base-margin) !important; margin-bottom: quarter($base-margin) !important; }
%me-- { margin-right:  quarter($base-margin) !important; margin-left:   quarter($base-margin) !important; }
</code></pre>
</div>


<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Margins Small</h2>
<pre><code class=" language-sass" data-lang="scss">%m-  { margin:        half($base-margin) !important; }
%mt- { margin-top:    half($base-margin) !important; }
%mr- { margin-right:  half($base-margin) !important; }
%mb- { margin-bottom: half($base-margin) !important; }
%ml- { margin-left:   half($base-margin) !important; }
%me- { margin-top:    half($base-margin) !important; margin-bottom: half($base-margin) !important; }
%ms- { margin-right:  half($base-margin) !important; margin-left:   half($base-margin) !important; }
</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Margins Large</h2>
<pre><code class=" language-sass" data-lang="scss">%m_x  { margin:        double($base-margin) !important;  }
%mt_x { margin-top:    double($base-margin) !important;  }
%mr_x { margin-right:  double($base-margin) !important;  }
%mb_x { margin-bottom: double($base-margin) !important;  }
%ml_x { margin-left:   double($base-margin) !important;  }
%me_x { margin-top:    double($base-margin) !important; margin-bottom:  double($base-margin) !important; }
%ms_x { margin-right:  double($base-margin) !important; margin-left:    double($base-margin) !important; }
</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Margins Huge</h2>
<pre><code class=" language-sass" data-lang="scss">%m_xx  { margin:        quadruple($base-margin) !important;  }
%mt_xx { margin-top:    quadruple($base-margin) !important;  }
%mr_xx { margin-right:  quadruple($base-margin) !important;  }
%mb_xx { margin-bottom: quadruple($base-margin) !important;  }
%ml_xx { margin-left:   quadruple($base-margin) !important;  }
%ms_xx { margin-top:    quadruple($base-margin) !important; margin-bottom: quadruple($base-margin) !important; }
%me_xx { margin-right:  quadruple($base-margin) !important; margin-left:   quadruple($base-margin) !important; }
</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Margins None</h2>
<pre><code class=" language-sass" data-lang="scss">%m0  { margin:        0 !important; }
%mt0 { margin-top:    0 !important; }
%mr0 { margin-right:  0 !important; }
%mb0 { margin-bottom: 0 !important; }
%ml0 { margin-left:   0 !important; }
%me0 { margin-top:    0 !important; margin-bottom: 0 !important; }
%ms0 { margin-right:  0 !important; margin-left:   0 !important; }
</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Paddings</h2>
<pre><code class=" language-sass" data-lang="scss">%p  { padding:        $base-padding !important; }
%pt { padding-top:    $base-padding !important; }
%pr { padding-right:  $base-padding !important; }
%pb { padding-bottom: $base-padding !important; }
%pl { padding-left:   $base-padding !important; }
%pe { padding-top:    $base-padding !important; padding-bottom: $base-padding !important; }
%ps { padding-right:  $base-padding !important; padding-left:   $base-padding !important; }
</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Paddings Tiny</h2>
<pre><code class=" language-sass" data-lang="scss">%p--  { padding:        quarter($base-padding) !important; }
%pt-- { padding-top:    quarter($base-padding) !important; }
%pr-- { padding-right:  quarter($base-padding) !important; }
%pb-- { padding-bottom: quarter($base-padding) !important; }
%pl-- { padding-left:   quarter($base-padding) !important; }
%pe-- { padding-top:    quarter($base-padding) !important; padding-bottom: quarter($base-padding) !important; }
%ps-- { padding-right:  quarter($base-padding) !important; padding-left:   quarter($base-padding) !important; }
</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Paddings Small</h2>
<pre><code class=" language-sass" data-lang="scss">%p-  { padding:        half($base-padding) !important; }
%pt- { padding-top:    half($base-padding) !important; }
%pr- { padding-right:  half($base-padding) !important; }
%pb- { padding-bottom: half($base-padding) !important; }
%pl- { padding-left:   half($base-padding) !important; }
%pe- { padding-top:    half($base-padding) !important; padding-bottom: half($base-padding) !important; }
%ps- { padding-right:  half($base-padding) !important; padding-left:   half($base-padding) !important; }

</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Paddings Large</h2>
<pre><code class=" language-sass" data-lang="scss">%p_x  { padding:        double($base-padding) !important; }
%pt_x { padding-top:    double($base-padding) !important; }
%pr_x { padding-right:  double($base-padding) !important; }
%pb_x { padding-bottom: double($base-padding) !important; }
%pl_x { padding-left:   double($base-padding) !important; }
%pe_x { padding-top:    double($base-padding) !important; padding-bottom: double($base-padding) !important; }
%ps_x { padding-right:  double($base-padding) !important; padding-left:   double($base-padding) !important; }
</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Paddings Huge</h2>
<pre><code class=" language-sass" data-lang="scss">%p_xx  { padding:        quadruple($base-padding) !important; }
%pt_xx { padding-top:    quadruple($base-padding) !important; }
%pr_xx { padding-right:  quadruple($base-padding) !important; }
%pb_xx { padding-bottom: quadruple($base-padding) !important; }
%pl_xx { padding-left:   quadruple($base-padding) !important; }
%pe_xx { padding-top:    quadruple($base-padding) !important; padding-bottom: quadruple($base-padding) !important; }
%ps_xx { padding-right:  quadruple($base-padding) !important; padding-left:   quadruple($base-padding) !important; }
</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Paddings None</h2>
<pre><code class=" language-sass" data-lang="scss">%p0  { padding:        0 !important; }
%pt0 { padding-top:    0 !important; }
%pr0 { padding-right:  0 !important; }
%pb0 { padding-bottom: 0 !important; }
%pl0 { padding-left:   0 !important; }
%pe0 { padding-top:    0 !important; padding-bottom: 0 !important; }
%ps0 { padding-right:  0 !important; padding-left:   0 !important; }
</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Word breaking</h2>
    <p>Break strings when their length exceeds the width of their container.</p>
    <pre><code class=" language-sass" data-lang="scss">%u-textBreak</code></pre>
</div>


<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Inherit Color</h2>
    <pre><code class=" language-sass" data-lang="scss">%u-textInheritColor</code></pre>
</div>


<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Font Kerning</h2>
    <pre><code class=" language-sass" data-lang="scss">%u-textKern</code></pre>
</div>


<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Prevent Whitespace Wrapping</h2>
    <pre><code class=" language-sass" data-lang="scss">%u-textNoWrap</code></pre>
</div>


<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Truncate Text</h2>
    <pre><code class=" language-sass" data-lang="scss">%u-textTruncate</code></pre>
</div>


<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Small Text</h2>
    <pre><code class=" language-sass" data-lang="scss">%u-textSize-small</code></pre>
</div>

<div class="panel  panel-default  p  markdown-body">
    <h2 class="styleguide-title">Capital Case Element</h2>
    <pre><code class=" language-sass" data-lang="scss">.u-posAbsolute</code></pre>
</div>
