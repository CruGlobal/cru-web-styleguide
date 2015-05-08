---
layout: page
type: page-styleguide-components
title: Popovers
page-class: page--ui-popovers
excerpt: Add small overlays of content, like those on the iPad, to any element for housing secondary information. Popovers whose both title and content are zero-length are never displayed.
---

## Contents
* Will be replaced with the ToC, excluding the "Contents" header
{:toc}


{% example html %}
<button type="button" class="btn  btn-subtle" data-container="body" data-toggle="popover" data-placement="left" data-content="Vivamus sagittis lacus vel augue laoreet rutrum faucibus.">
  Popover on left
</button>

<button type="button" class="btn  btn-subtle" data-container="body" data-toggle="popover" data-placement="top" data-content="Vivamus sagittis lacus vel augue laoreet rutrum faucibus.">
  Popover on top
</button>

<button type="button" class="btn  btn-subtle" data-container="body" data-toggle="popover" data-placement="bottom" data-content="Vivamus
sagittis lacus vel augue laoreet rutrum faucibus.">
  Popover on bottom
</button>

<button type="button" class="btn  btn-subtle" data-container="body" data-toggle="popover" data-placement="right" data-content="Vivamus sagittis lacus vel augue laoreet rutrum faucibus.">
  Popover on right
</button>
{% endexample %}
