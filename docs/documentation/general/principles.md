---
layout: page
type: page-documentation-general
title: Development Principles
excerpt:
---
<p class="mb-">Cru has a huge codebase and this ultimately dictates many of the decisions we make around the front end architecture and day-to-day feature development.</p>

- Leave code in a better state than you found it
- Reuse as much as possible: technologies and components
- The entire code base should look like one person wrote it
- Keep it simple
- Ensure we can pivot away from a dependency/pattern


#### Resuse as much code as possible
Our codebase is too large to hold in your head and there is no return in trying to do so. We have to break down the functionality of into simple modules which we compose into robust sites.


#### Keep things simple
More than anything, please try to follow existing patterns as much as possible. Inconsistency soon manifests as complexity and then technical debt. What we are aiming to build is a maintainable platform where developers can move between applications with very little up-front learning required. [The best tool for the job, isn’t always](https://medium.com/@bentlegen/the-best-tool-for-the-job-isnt-always-6ed364f3f775) by Ben Vinegar covers this concept perfectly.

Sometimes reusing code will take more initial work, but it shouldn't be avoided. When building new features, try to identify reusable parts which can be abstracted into Crubrand to help other developers. Features not in Crubrand are inherently harder to find and thus reuse.


#### Ensure that we can pivot

When making broad decisions, trust that your expertise means you're correct now, but realize that things will change and we may possibly need to pivot away from what you decide on. There is a cost to removing something from the codebase which far outweighs the cost of adding it.

Everything is up for discussion, but pivoting on such a huge code base is a slow process so it's always worth spending the extra time to consider how deeply we would be tied into the decision and how quickly we could change course.
