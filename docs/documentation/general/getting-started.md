---
layout: page
type: page-documentation-general
title: Getting Started
---

<p class="mb-">If you already have an existing `bower.json` file, run the following command:</p>

<pre><code>bower install --save crubrand</code></pre>

Otherwise, create a bower project. If you are not sure what to enter in the prompts, use the default values (by hitting return):

<pre><code>bower init</code></pre>

After installing the project, install crubrand as a dependency:

<pre><code>bower install --save crubrand</code></pre>

You can change the release number to meet your needs. For more information about release numbers see [this project](this project).

When needed you can update cruband using Bower. You may need to change the release number in the `bower.json` file if you are updating to a new version.
<pre><code>bower update</code></pre>

Once installed, `@import` into your project's main scss file:
<pre><code>@import "bower_components/crubrand/crubrand";</code></pre>

You can [see a sample project](https://github.com/CruGlobal/crubrand-web-template) with examples of a basic and more involved way to use crubrand
