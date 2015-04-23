---
layout: page
title: Typography
---

This lists the primary and secondary color palettes as described in the Brand Guidelines PDF and in [_colors.scss](https://github.com/CruGlobal/crubrand/blob/master/variables/_colors.scss).

## Contents

* Will be replaced with the ToC, excluding the "Contents" header
{:toc}

## Headings

{% example html %}
<h1>Dapibus Magna Ornare Tellus</h1>
<h2>Dapibus Magna Ornare Tellus</h2>
<h3>Dapibus Magna Ornare Tellus</h3>
<h4>Dapibus Magna Ornare Tellus</h4>
<h5>Dapibus Magna Ornare Tellus</h5>
<h6>Dapibus Magna Ornare Tellus</h6>
{% endexample %}

## Body text

{% example html %}
<p>Donec id elit non mi porta gravida at eget metus. Etiam porta sem malesuada magna mollis euismod. Maecenas sed diam eget risus varius blandit sit amet non magna. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor. Cras mattis consectetur purus sit amet fermentum. Etiam porta sem malesuada magna mollis euismod. Donec ullamcorper nulla non metus auctor fringilla.</p>
<p>Nullam id dolor id nibh ultricies vehicula ut id elit. Cras justo odio, dapibus ac facilisis in, egestas eget quam. Aenean lacinia bibendum nulla sed consectetur. Etiam porta sem malesuada magna mollis euismod. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Cras justo odio, dapibus ac facilisis in, egestas eget quam.</p>
{% endexample %}


## Inline text elements

{% example html %}
<p>You can use the mark tag to <mark>highlight</mark> text.</p>
<p><del>This line of text is meant to be treated as deleted text.</del></p>
<p><s>This line of text is meant to be treated as no longer accurate.</s></p>
<p><ins>This line of text is meant to be treated as an addition to the document.</ins></p>
<p><u>This line of text will render as underlined</u></p>
<p><small>This line of text is meant to be treated as fine print.</small></p>
<p><strong>This line rendered as bold text.</strong></p>
<p><em>This line rendered as italicized text.</em></p>
{% endexample %}

## Blockquotes

Wrap `<blockquote>` around any <abbr title="HyperText Markup Language">HTML</abbr> as the quote. For straight quotes, we recommend a `<p>`.

{% example html %}
<blockquote>
  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.
</blockquote>
{% endexample %}

## Pullquotes

{% example html %}
<blockquote class="pullquote"><em>But you can’t take a part of truth and make it the whole.</em></blockquote>
{% endexample %}
