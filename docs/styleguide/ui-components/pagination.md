---
layout: page
type: page-styleguide-components
title: Pagination
---

Provide pagination links for your site or app with the multi-page pagination component, or the simpler [pager alternative](#pager).


## Contents

* Will be replaced with the ToC, excluding the "Contents" header
{:toc}

## Default Pagination

Simple pagination, great for apps and search results. The large block is hard to miss, easily scalable, and provides large click areas.

{% example html %}
<nav>
    <ul class="pagination">
        <li>
            <a href="#" aria-label="Previous" class="pagination-prev">Previous</a>
        </li>
        <li>
            <a href="#">1</a>
        </li>
        <li>
            <a href="#">2</a>
        </li>
        <li>
            <a href="#">3</a>
        </li>
        <li>
            <a href="#">4</a>
        </li>
        <li>
            <a href="#">5</a>
        </li>
        <li>
            <a href="#" aria-label="Next"  class="pagination-next">Next</a>
        </li>
    </ul>
</nav>
{% endexample %}


### Disabled and active states

Links are customizable for different circumstances. Use `.disabled` for unclickable links and `.active` to indicate the current page.

{% example html %}
<nav>
    <ul class="pagination">
        <li class="disabled ">
            <a href="#" aria-label="Previous" class="pagination-prev">Previous</a>
        </li>
        <li class="active">
            <a href="#">1</a>
        </li>
        <li>
            <a href="#">2</a>
        </li>
        <li>
            <a href="#">3</a>
        </li>
        <li>
            <a href="#">4</a>
        </li>
        <li>
            <a href="#">5</a>
        </li>
        <li>
            <a href="#" aria-label="Next"  class="pagination-next">Next</a>
        </li>
    </ul>
</nav>
{% endexample %}


## Pager

Quick previous and next links for simple pagination implementations with light markup and styles. It's great for simple sites like blogs or magazines.

{% example html %}
<nav>
    <ul class="pager">
        <li>
            <a href="#" class="pager-prev">Previous</a>
        </li>
        <li>
            <a href="#" class="pager-next">Next</a>
        </li>
    </ul>
</nav>
{% endexample %}


### Aligned links

Alternatively, you can align each link to the sides:

{% example html %}
<nav>
    <ul class="pager">
        <li class="previous">
            <a href="#" class="pager-prev">Older</a>
        </li>
        <li class="next">
            <a href="#" class="pager-next">Newer</a>
        </li>
    </ul>
</nav>
{% endexample %}


### Optional disabled state

Pager links also use the general `.disabled` utility class from the pagination.


{% example html %}
<nav>
    <ul class="pager">
        <li class="previous disabled">
            <a href="#" class="pager-prev">Older</a>
        </li>
        <li class="next">
            <a href="#" class="pager-next">Newer</a>
        </li>
    </ul>
</nav>
{% endexample %}
