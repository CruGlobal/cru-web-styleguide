---
layout: page
title: Overview
---

Get the lowdown on the key pieces of Bootstrap's infrastructure, including our approach to better, faster, stronger web development.

## Contents

* Will be replaced with the ToC, excluding the "Contents" header
{:toc}

## HTML5 doctype

Bootstrap makes use of certain HTML elements and CSS properties that require the use of the HTML5 doctype. Include it at the beginning of all your projects.

{% highlight html %}
<!DOCTYPE html>
<html lang="en">
  ...
</html>
{% endhighlight %}

## Mobile first

Bootstrap is mobile first. Mobile first styles can be found throughout the entire library instead of in separate files.

To ensure proper rendering and touch zooming, add the viewport meta tag to your `<head>`.

{% highlight html %}
<meta name="viewport" content="width=device-width, initial-scale=1">
{% endhighlight %}

## Typography and links

Crubrand sets the basic global display, typography, and link styles.
More details can be found in the following sections [Type](/Links/), [Links](/links/).
