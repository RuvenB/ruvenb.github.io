---
layout: post
title:  "Content from CSS"
date:   2021-12-05 19:36:01 +0100
categories: css javascript
---
Normally I use `:before` only to add a List-Item or to add a picture in front, but
there has to be more.

I try to see how much content you can put in `:before` und `:after` css content.
The second thing I try here is how to update CSS per javascript.

Following are a few empty divs, which are filled per css. With the button you can toggle
between two css files, which set content to the divs.

{% include contentFromCss.html %}

# Why do this?
- because you can
- you don't want make it easy to copy your content

# Why you shouldn't do this?
- your blind pal google can't read the content
- accessibility in general is down
- it's not that easy to add content
    - but you could write a tool for this, of course
- not everything ist possible there
    - links or buttons aren't
        - I guess there is more
    - tables will be a pain to create
        - but you have written a tool by then to create them from your markdown, right?