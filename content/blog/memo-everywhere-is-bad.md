---
title: Memoizing every react component is bad
date: '2021-10-06T18:49:22.597Z'
description: Just a random thought i had while travelling.
---

I suddenly had a thought, why not to make a build time plugin to add memo to every single component. Obviously , this is not something only i though of. I saw a good discussion in a issue of facebook/react github repo.And with tweet, i understood memo() everywhere is bad.  

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">Shallow comparisons aren’t free. They’re O(prop count). And they only buy something if it bails out. All comparisons where we end up re-rendering are wasted.<br><br>Why would you expect always comparing to be faster? Considering many components always get different props.</p>&mdash; Dan (@dan_abramov) <a href="https://twitter.com/dan_abramov/status/1095661142477811717?ref_src=twsrc%5Etfw">February 13, 2019</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

