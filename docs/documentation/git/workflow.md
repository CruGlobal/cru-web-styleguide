---
layout: page
type: page-documentation-git
title: Workflow
---

<p class="mb-">This is the workflow you should adopt for a typical feature.</p>

- Get the latest version of master

<pre>
<code>git pull origin master</code>
</pre>

- Create your own feature branch, prefixed by your initials. Branches should be scoped to one feature and short-lived.

<pre>
<code>git checkout -b jd-feature</code>
</pre>

- Discuss the feature with another developer, they should eventually review your code.

- Do some work

- Push to a remote branch, rebasing beforehand if you have redundant commits which should be squashed

- Create a Pull Request

- Ask/assign another developer to review the code. You should talk with them about the pull request whenever possible.

- Reply to comments and make amends

- The reviewer should merge into master once the request receives a +1

- Delete your feature branch
