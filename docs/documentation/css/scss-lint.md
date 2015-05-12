---
layout: page
type: page-documentation-css
title: SCSS Lint
page-class: page--documentation-css
excerpt: We use <a href="https://github.com/brigade/scss-lint">scss-lint</a> to ensure our code follows the same general principles and to keep everything looking the same.  
---

#### Requirements

- Ruby 1.9.3+
- Sass 3.4.1+ (scss-lint 0.27.0 was the last version to support Sass 3.3)
- Files you wish to lint must be written in SCSS (not Sass) syntax

#### Installation

<pre><code>gem install scss_lint</code></pre>


#### Usage

Run `scss-lint` from the command-line by passing in a directory (or multiple directories) to recursively scan:

<pre><code>scss-lint app/assets/stylesheets/</code></pre>

You can also specify a list of files explicitly:

<pre><code>scss-lint app/assets/stylesheets/**/*.css.scss</code></pre>


See [the documentation](https://github.com/brigade/scss-lint) for more information on configuration and advanced usage.


#### Our rules

View [a live `scss-lint.yml` file](https://github.com/CruGlobal/crubrand/blob/master/.scss-lint.yml).

- Space before !important, not after. [BangFormat]

- Use `border: 0` instead of `border: none`. [BorderZero]

- Do not use color keywords — such as `green` instead of `#008000`. [ColorKeyword]

- Do not leave `@debug` statements in your code. Clean up after yourself. [DebugStatement]

- Do not define any property more than once within a single rule set. [DuplicateProperty]

- Put `@else` on a new line from the curly brace it follows. [ElsePlacement]

- Include an empty line between all statements — i.e. rule sets, at-rules, and Sass directives. Even the nested ones. Spaces help people, and people are important. (Variable definitions are like properties and don’t need to be spaced.) [EmptyLineBetweenBlocks]

- Do not leave empty rule sets in your code. [EmptyRule]

- End each file with an empty newline. [FinalNewline]

- Use the shortest possible hex value. `#fff` instead of `#ffffff`. [HexLength]

- Use lowercase letters inside hex values. `#fff` instead of `#FFF`. [HexNotation]

- Only use three or six hexidecimal characters. [HexValidation]

- Never use ID selectors in your stylesheets. Find another way. (No, this is not “throwing out the baby with the bath water”. This is “not pooping in the bath”.) [IdSelector]

- Do not include leading underscores or filename extensions in the basenames of SCSS files that you @import. `@import generic/reset` instead of `@import horse/_donkey.scss`;. [ImportPath]

- Indent using 4 spaces. Or soft-tabs. [Indentation]

- Do include an unnecessary leading zero before decimal values less than 1. `0.5em` instead of `.5em`. It improves readability. [LeadingZero]

- Ensure that there are not repeat selectors, with different styles in a single stylesheet. [MergeableSelector]

- Do not nest selectors more than 3 levels deep. Zero levels of nesting is best, of course. One level is often handy, and arguably helps organize some common code (especially pseudo-classes and pseudo-elements). Two or three raises eyebrows and specificity. More invites (induces?) disaster. [NestingDepth]

- `@extend` placeholders only. This practice will help prevent some common `@extend`-related mistakes and misunderstandings. [PlaceholderInExtend]

- Do not misspell properties. In fact, do not misspell anything, ever. [PropertySpelling]

- Do not qualify type selectors. Better yet, don’t use them at all, if possible: just use classes. [QualifyingElement]

- Do not chain more than three simple selectors. In almost every case, one simple selector is best (that is, no chaining, flat specificity, world peace). Some situations call for two. But let’s just draw the line at three. Find another way. [SelectorDepth]

- Use shorthand properties when you can. But only when necessary [Shorthand]

- Include a line break between each declaration. Keep declarations isolated: that way you can monitor and discipline them more easily. [SingleLinePerProperty]

- Include a line break between each selector in a group. [SingleLinePerSelector]

- Include spaces after commas and colons, not before. As in written English. [SpaceAfterComma, SpaceAfterPropertyColon, SpaceAfterPropertyName]

- Include a single space between selectors and the curly braces that begin declaration blocks. [SpaceBeforeBrace]

- Do not include spaces between parentheses and parenthesized. As in written English. [SpaceBetweenParens]

- Use double quotation marks. [StringQuotes]

- Do not include unnecessary trailing zeros after a decimal point. `2em` instead of `2.0em`. [TrailingZero, UnnecessaryMantissa]

- Include quotation marks around URLs. SCSS-Lint documentation [explains why](https://github.com/causes/scss-lint/blob/master/lib/scss_lint/linter/README.md#urlquotes). [UrlQuotes]

- Do not type vendor prefixes. You have too much life to live. We use Bourbon mixins. [VendorPrefixes]

- Do not include units on zero values. It could be zero of anything: we don’t have to know. [ZeroUnit]
