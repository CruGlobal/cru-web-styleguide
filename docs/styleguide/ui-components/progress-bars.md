---
layout: page
type: page-styleguide-components
title: Progress Bars
excerpt: Provide up-to-date feedback on the progress of a workflow or action with simple yet flexible progress bars.
---

<div class="docs-callout docs-callout-danger" id="callout-progress-animation-css3">
    <h4 id="cross-browser-compatibility">Cross-browser compatibility<a class="anchorjs-link" href="#cross-browser-compatibility"><span class="anchorjs-icon"></span></a></h4>
    <p>Progress bars use CSS3 transitions and animations to achieve some of their effects. These features are not supported in Internet Explorer 9 and below or older versions of Firefox. Opera 12 does not support animations.</p>
</div>


## Contents

* Will be replaced with the ToC, excluding the "Contents" header
{:toc}

## Basic example

{% example html %}
<div class="progress">
  <div class="progress-bar" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" style="width: 60%;">
    <span class="u-hiddenVisually">60% Complete</span>
  </div>
</div>
{% endexample %}


## With label
Remove the `<span>` with `.sr-only` class from within the progress bar to show a visible percentage.

{% example html %}
    <div class="progress">
      <div class="progress-bar" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" style="width: 60%;">
        60%
      </div>
    </div>
{% endexample %}


To ensure that the label text remains legible even for low percentages, consider adding a `min-width` to the progress bar.

{% example html %}
    <div class="progress">
      <div class="progress-bar" role="progressbar" aria-valuenow="0" aria-valuemin="0" aria-valuemax="100" style="min-width: 2em;">
        0%
      </div>
    </div>
    <div class="progress">
      <div class="progress-bar" role="progressbar" aria-valuenow="2" aria-valuemin="0" aria-valuemax="100" style="min-width: 2em; width: 2%;">
        2%
      </div>
    </div>
{% endexample %}


## Striped

Uses a gradient to create a striped effect. Not available in IE9 and below.

{% example html %}
<div class="progress">
  <div class="progress-bar progress-bar-striped" role="progressbar" aria-valuenow="40" aria-valuemin="0" aria-valuemax="100" style="width: 40%">
    <span class="u-hiddenVisually">40% Complete (success)</span>
  </div>
</div>
{% endexample %}


## Animated

{% example html %}
<div class="progress">
  <div class="progress-bar progress-bar-striped active" role="progressbar" aria-valuenow="45" aria-valuemin="0" aria-valuemax="100" style="width: 45%">
    <span class="u-hiddenVisually">45% Complete</span>
  </div>
</div>
{% endexample %}
