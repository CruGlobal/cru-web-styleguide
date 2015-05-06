---
layout: page
type: page-documentation-css
title: CSS
page-class: page--documentation-css
---
<p>Cru uses <a href="http://sass-lang.com/">SCSS</a> for CSS generation</p>
<p>Cru's naming conventions are adapted from the work being done in Nicolas Gallagher's <a href="https://github.com/suitcss/suit/tree/master/doc">SUITCSS</a>. Which is to say, it relies on structured, meaningful class names. This is to help work around the current limits of applying CSS to the DOM (i.e., the lack of style encapsulation) and to better communicate the relationships between classes. We also heavily rely on the principles taught by Harry Roberts in <a href="http://cssguidelin.es/">Guideline.es</a>.</p>
<p>We are currently using <a href="http://getbootstrap.com/">Bootstrap</a> as our foundation because it does much of the heavy lifting for us. We have adapted it to best fit our uses and eliminate extraneous code. <a href="https://github.com/CruGlobal/crubrand">Our basic build can be installed as a bower package</a>, which includes Bootstrap, with our variable overrides and other changes.</p>
<p>Our primary goal is to create a scalable, maintainable and reusable css. Here is a <a href="https://github.com/davidtheclark/scalable-css-reading-list">Scalable CSS Reading List</a> take a look.</p>

## Contents

* Will be replaced with the ToC, excluding the "Contents" header
{:toc}

## A quick word about the dangers of SASS

While SASS can be a powerful tool in the right hands, in the wrong hands you can end up with
selectors like this:


    body.getaways-gallery-gig .page_header #filters #categories_filter
    .pane .categories_container .categories ul li.selectBox-selected a {
    color: #333;
    }


Because of the ease of nesting in preprocessors like SASS, inexperienced devs
will often nest like crazy without understanding the ramifications on the
compiled code. This adds a ton of unnecessary specificity that requires the
same selector to override or worse, using `!important`. (Sometimes times devs will even resort
to inline styles! Ewww.)


## Document Anatomy

No matter the document, we must always try and keep a common formatting. This means consistent
commenting, consistent syntax and consistent naming.

### General
Limit your stylesheets to a maximum 80 character width where possible. Exceptions may be gradient
syntax and URLs in comments. There's nothing we can do about those.

### Single file vs. many files

While some people prefer to work with single, large files we choose not to do this. We have chosen
to split up our stylesheets into lots of tiny includes as this allows each file to be more
scannable and focused.

### Table of contents

At the top of stylesheets, a table of contents will detail the sections contained in the document,
for example:

    /*------------------------------------*\
        #CONTENTS
    \*------------------------------------*/
    /**
     * CONTENTS............It's what you are reading
     * RESET...............Set our reset defaults
     * FONT-FACE...........Import brand font files
     */

This will tell the next developer(s) exactly what they can expect to find in this file. Each item
in the table of contents maps directly to a section title.

Since we are working across multiple files then each item in the table of contents will map to an
include which pulls that section in.

### Section titles

The table of contents would be of no use unless it had corresponding section titles. Denote a
section thus:

    /*------------------------------------*\
        #RESET
    \*------------------------------------*/

The `#` prefixing the name of the section allows us to run a find ([Cmd|Ctrl]+F) for
`#[SECTION-NAME]` and **limit our search scope to section titles only**.

### Comments

Code is written and maintained by people. Ensure your code is descriptive, well commented, and
approachable by others. Great code comments convey context or purpose. Do not simply reiterate a
component or class name.

Be sure to write in complete sentences for larger comments and succinct phrases for general notes.

**Bad Example:**

    /* Modal header */
    .modal-header {
      ...
    }


**Good Example:**

    /* Wrapping element for .modal-title and .modal-close */
    .modal-header {
      ...
    }



## File Structure

The typical file structure of a project will look like:


    bower_components/
    ├── crubrand/
    │   ├── bootstrap-variations/
    │   ├── bourbon/
    │   ├── components/
    │   ├── elements/
    │   ├── generic/
    │   ├── ie/
    │   ├── variables/
    │   ├── _crubrand.scss
    │   ├── _overrides.scss
    │   └──_settings.scss

    [projectname]-scss/
    ├── bootstrap-replacement/
    │   ├── ...
    │   ├── ...
    ├── ie/
    │   ├── ...
    │   └── ...
    ├── ...
    ├── ...
    ├── projectname.ie.scss
    └── projectname.scss


## Declarations

### Property Order

Properties should be organized in the following order:

  1. Extends
  2. Empty Mixins
  3. Positioning
  4. Display and Box Model
  5. Color
  6. Text
  7. Other
  8. Mixins
  9. Media Queries
  10. Nested Properties.



    .selector {
      /* Extend */
      @extend %component;

      @include clearfix;

      /* Positioning */
      position: absolute;
      z-index: 10;
      top: 0;
      right: 0;

      /* Display & Box Model */
      display: inline-block;
      overflow: hidden;
      box-sizing: border-box;
      width: 100px;
      height: 100px;
      padding: 10px;
      border: 10px solid #333;
      margin: 10px;

      /* Color */
      background: #000;
      color: #fff

      /* Text */
      font-family: sans-serif;
      line-height: 1.4;
      text-align: right;

      /* Other */
      cursor: pointer;

      /* Mixins */
      @include font-size(16px);

      /* Media query mixin */
      @include mq (800px) {
        ...
      }

      .selector-child{
        ...
      }
    }


### Single Declarations

In instances where a rule set includes only one declaration, consider removing line breaks for
readability and faster editing. Any rule set with multiple declarations should be split to separate
lines.

The key factor here is error detection -- e.g., a CSS validator stating you have a syntax error on
Line 183. With a single declaration, there's no missing it. With multiple declarations, separate
lines is a must for your sanity.

    /* Single declarations on one line */
    .one-third { width: 33.333%; }
    .one-half { width: 50%; }
    .one-whole { width: 100%; }

    /* Multiple declarations, one per line */
    .sprite {
      display: inline-block;
      width: 16px;
      height: 15px;
      background-image: url(../img/sprite.png);
    }

### Shorthand Notation

Strive to limit use of shorthand declarations to instances where you must explicitly set all the
available values. Common overused shorthand properties include:

  * padding
  * margin
  * font
  * background
  * border
  * border-radius

Often times we don't need to set all the values a shorthand property represents. For example, HTML
headings only set top and bottom margin, so when necessary, only override those two values.
Excessive use of shorthand properties often leads to sloppier code with unnecessary overrides and
unintended side effects.

The Mozilla Developer Network has [a great article on shorthand properties](https://developer.mozilla.org/en-US/docs/Web/CSS/Shorthand_properties) for those
unfamiliar with notation and behavior.


**Bad Example**

    .element {
      margin: 0 0 10px;
      background: red;
      background: url("image.jpg");
      border-radius: 3px 3px 0 0;
    }

**Good Example**

    .element {
      margin-bottom: 10px;
      background-color: red;
      background-image: url("image.jpg");
      border-top-left-radius: 3px;
      border-top-right-radius: 3px;
    }


## Formatting
The following are some high level page formatting style rules.

### Spacing
CSS rules should be comma separated but live on new lines:

**Correct:**

    .content,
    .content-edit {
      ...
    }

**Incorrect:**

    .content, .content-edit {
      ...
    }

CSS blocks should be separated by a single new line. Not two. Not 0.

**Correct:**

    .content {
      ...
    }

    .content-edit {
      ...
    }

**Incorrect:**

    .content {
      ...
    }
    .content-edit {
      ...
    }

### Whitespace and Punctuation

- Indent using 4 soft tabs. [Indentation]

- End each file with an empty newline. After all, you're not an animal, are you? [FinalNewline]

- Include an empty line between all statements i.e. rule sets, at-rules, and Sass directives.
  Even the nested ones. Spaces help people, and people are important. (Variable definitions are
  like properties and don't need to be spaced.) [EmptyLineBetweenBlocks]

- Include spaces after commas and colons, not before. As in written English. [SpaceAfterComma, SpaceAfterPropertyColon,SpaceAfterPropertyName]

- Do not include spaces between parentheses and parenthesized. As in written English. [SpaceBetweenParens]

- Use double quotation marks. Quotes are optional in CSS and LESS. We use double quotes as it
  is visually clearer that the string is not a selector or a style property. [StringQuotes]

- End every declaration with a semicolon, with no whitespace in front of it. [TrailingSemicolon]


## Javascript

syntax: `js-<targetName>`

JavaScript-specific classes reduce the risk that changing the structure or theme of components
will inadvertently affect any required JavaScript behavior and complex functionality. It is
not necessary to use them in every case, just think of them as a tool in your utility belt. If
you are creating a class, which you don't intend to use for styling, but instead only as a
selector in JavaScript, you should probably be adding the `js-` prefix. In practice this looks
like this:


    <a href="/login" class="btn  btn-primary  js-login"></a>


**Again, JavaScript-specific classes should not, under any circumstances, be styled**.


## Utilities

syntax: `u-<utlitityName>`

Utility classes are low-level structural and positional traits. Utilities can be applied directly
to any element; multiple utilities can be used together; and utilities can be used alongside
component classes.

Utilities exist because certain CSS properties and patterns are used frequently.
For example: floats, containing floats, vertical alignment, text truncation. Relying on utilities
can help to reduce repetition and provide consistent implementations.

Utilities are complete single responsibility rules which have a very specific and targeted task.
It is also quite common for these rules' declarations to carry `!important` so as to guarantee
they beat other less specific ones. They do one thing in a very heavy-handed and inelegant way.
They are to be used as a last resort when no other CSS hooks are available, or to tackle
completely unique circumstances, e.g. using `.u-text-center` to centrally align one piece of text
once and once only. They are only one step away from inline styles, so should be used sparingly.

Because of their heavy-handed approach, their global reusability, and their exceptional use-case,
it is incredibly important that we signal Utilities to other developers. We do not want anyone
trying to bind onto these in future selectors.

### u-utilityname

Utilities must be prefixed with a `u-` namespace. By using a namespace, we can introduce a simple
and unbreakable rule: if it begins with `u-`, never reassign to it.


## Components

Syntax: `<componentName>[--modifierName|-descendantName]`

This has several benefits when reading and writing HTML and CSS:

* It helps to distinguish between the classes for the root of the component, descendent elements,
  and modifications.
* It keeps the specificity of selectors low.
* It helps to decouple presentation semantics from document semantics.

We use a modified version of the SUIT BEM naming convention.

    /**
     * The top-level â€˜Blockâ€™ of a component.
     */
    .modal {}

      /**
       * An â€˜Elementâ€™ that is a part of the larger Block.
       */
      .modal-title {}

    /**
     * A â€˜Modifierâ€™ of the Block.
     */
    .modal--large {}


In our CSS, this naming isn't all that useful, but when we see it in out HTML we get a much
better view of what's going on:


    <div class="modal  modal--large">

      <h1 class="modal-title">Sign into your account</h1>

      <div class="modal-content">
        <form class="form-login">
        </form>
      </div>

    </div>

We can see from this that we have a number of classes all relating to our `.modal`, and a class
of `.form-login` which begins a brand new context.

Being able to glean this level of information from our classes in our markup actually tells us
quite a lot about the corresponding CSS, and also about how and why they interact with each other
in the way they do. It also tells us about how we should (or should not) reuse these classes
elsewhere in the DOM: `.modal--large`, `.modal-title`, and `.modal-content` all have a dependency
on `.modal`, and therefore cannot be used without that .modal class also being present.

### componentName

The component's name must be written in camel case. This is the top-level of a component.

    .myComponent {
        /* ... */
    }


    <div class="myComponent">
      ...
    </div>

### componentname--modifierName

A component modifier is a class that modifies the presentation of the base component in some form.
Modifier names must be written in camel case and be separated from the component name by two
hyphens. The class should be included in the HTML in addition to the base component class.


    /* Core button */
    .btn {
        /* ... */
    }

    /* Default button style */
    .btn--default {
        /* ... */
    }


    <div class="btn  btn--default">
      ...
    </div>

### componentname-descendantName

A component descendant is a class that is attached to a descendant node of a component. It's
responsible for applying presentation directly to the descendant on behalf of a particular
component. Descendant names must be written in camel case.


### is-stateOfComponent

Use `is/has-stateName`, depending on the context, for state-based modifications of components.
The state name must be Camel case. **Never style these classes directly; they should always
be used as an adjoining class.**

JS can add/remove these classes. This means that the same state names can be used in multiple
contexts, but every component must define its own styles for the state (as they are scoped to
the component).

    .dropdown {
      /* ... */
    }

    .dropdown.is-open {
      /* ... */
    }

    <ul class="dropdown  is-open">
      ...
    </ul>


## Variables

### colors

When implementing feature styles, you should only be using color variables provided by` _colors.scss`
found in <a href="https://github.com/CruGlobal/crubrand">crubrand</a>.

When adding a color variable to `_colors.scss`, using hex color units are preferred over RGB and RGBA,
named, HSL, or HSLA values. We also prefer to shorten hex values whenever possible

Color variables should use the naming convention `color-[nameOfColor]`

**Correct:**

    #fff;
    #3a3a3a;


**Incorrect:**

    #ffffff;
    rgb(50, 50, 50);
    rgba(50, 50, 50, 0.2);
    white;
    hsl(120, 100%, 50%);
    hsla(120, 100%, 50%, 1);


### z-index

Please use the z-index scale defined in `_z-index.scss` found in <a href="https://github.com/CruGlobal/crubrand">crubrand</a>.

`$zIndex-1 - $zIndex-9` are provided. Nothing should be higher then `$zIndex-9`.

<!--
### font-weight

### line-height

### letter-spacing


## Mixins


## Extends
-->


## Media Queries

Place media queries inside their relevant rule sets whenever possible. Don't bundle them all in a
separate stylesheet or at the end of the document. Doing so only makes it easier for folks to miss
them in the future. Here's a typical setup.

**Correct:**

    .componentName {
        @media (min-width: 480px) {
          /* ... */
        }
    }

**Incorrect:**

    @media (min-width: 480px) {
        .componentName{ /* ... */ }
        .anotherComponent{ /* ... */ }
    }



## Performance


### Specificity

Although in the name (cascading style sheets), cascading can introduce unnecessary performance
overhead for applying styles. Take the following example:

    ul.user-list li span a:hover { color: red; }


Styles are resolved during the renderer's layout pass. The selectors are resolved right to left,
exiting when it has been detected the selector does not match. Therefore, in this example every a
tag has to be inspected to see if it resides inside a span and a list. As you can imagine this
requires a lot of DOM walking and and for large documents can cause a significant increase in the
layout time. For further reading checkout: https://developers.google.com/speed/docs/best-practices/rendering#UseEfficientCSSSelectors

[The CSS Tricks article about selector performance](http://css-tricks.com/efficiently-rendering-css/)
should help explain the important concept of the key selector. Seemingly specific rules like
`.component-descendant-descendant div` are actual quite expensive in complex apps because rules
are read from right to left. It needs to look up all the divs first (which could be thousands) then
go up the DOM from there.

If we know we want to give all a elements inside the `.user-list` red on hover we can simplify
this style to:

    .user-list > a:hover {
      color: red;
    }

If we want to only style specific a elements inside `.user-list` we can give them a specific class:

    .user-list > .link-primary:hover {
      color: red;
    }


###Layouts and Paints

[Juriy Zaytsev's post on CSS profiling](http://perfectionkills.com/profiling-css-for-fun-and-profit-optimization-notes/)
profiles browsers on selector matching, layouts, paints, and parsing times of a complex app. It
confirms the theory that highly specific selectors are bad for big apps. Harry Roberts of CSS
Wizardry also wrote about [CSS selector performance](http://csswizardry.com/2011/09/writing-efficient-css-selectors/).

Layouts and paints can cause lots of performance damage. Be cautious with CSS3 features like
text-shadow, box-shadow, border-radius, and animations, [especially when used together](http://www.html5rocks.com/en/tutorials/speed/css-paint-times/). Trello wrote a big
blog post about performance [back in January 2014](http://blog.fogcreek.com/we-spent-a-week-making-trello-boards-load-extremely-fast-heres-how-we-did-it/).
Much of this was due to layout thrashing caused by JavaScript, but we cut out some heavy styles
like borders, gradients, and shadows, which helped a lot.
