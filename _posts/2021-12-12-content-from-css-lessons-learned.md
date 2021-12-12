---
layout: post
title:  "Content from CSS - lessons learned"
date:   2021-12-12 12:50:01 +0100
categories: css javascript
---

# Link works in the body
I always used `<link rel="stylesheet" href="...">` only in the head. It also works in the body.

# Href Change works immediate
In the last post we changed the href of the link by script. It works immediately.
I thought it would be neccessary to change the zoom-factor of the body or something like this.

# Next experiment
With clicking on the button we add 1,000,000 * 10 characters per `::after{content...}`.
If there is a limit, it is beyond my creative writing abilities.

Tested with Edge 96.0.1054.43 (Linewrapping sometimes out of place) and Firefox Nightly 97.0a1.

## Creating of String
I simply let Javascript write the content.

{% highlight javascript %}
const zeroPad = (num, places) => String(num).padStart(places, '0');
var l = [];
for(var i = 0; i<1000000; i++){
    l.push(zeroPad(i,9));
 }
 l.join(' ');
{% endhighlight %}

{% include contentFromCSS2.html %}