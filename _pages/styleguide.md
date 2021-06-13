---
layout: page
title: Style Guide
permalink: /styleguide/
image: '/images/120.jpg'
---

A paragraph looks like this — dolor amet cray stumptown fingerstache neutra food truck seitan poke cardigan waistcoat VHS snackwave celiac hella. Godard seitan shoreditch flexitarian next level trust fund man braid vegan listicle keytar bitters. Disrupt cray fashion axe unicorn lomo shaman poke glossier keffiyeh snackwave austin tattooed seitan hexagon lo-fi. Lumbersexual irony vaporware, butcher shaman.

***

## Headings by default:

# H1 For example
## H2 For example
### H3 For example
#### H4 For example
##### H5 For example
###### H6 For example

{% highlight markdown %}
## Heading first level
### Heading second level
#### Heading third level
{% endhighlight %}

***

## Lists

#### Ordered list example:

1. Poutine drinking vinegar bitters.
2. Coloring book distillery fanny pack.
3. Venmo biodiesel gentrify enamel pin meditation.
4. Jean shorts shaman listicle pickled portland.
5. Salvia mumblecore brunch iPhone migas.

{% highlight markdown %}
1. Order list item 1
2. Order list item 1
{% endhighlight %}

***

#### Unordered list example:

* Bitters semiotics vice thundercats synth.
* Literally cred narwhal bitters wayfarers.
* Kale chips chartreuse paleo tbh street art marfa.
* Mlkshk polaroid sriracha brooklyn.
* Pug you probably haven't heard of them air plant man bun.

{% highlight markdown %}
* Unordered list item 1
* Unordered list item 2
{% endhighlight %}

***

## Quotes

#### A quote looks like this:

> The longer I live, the more I realize that I am never wrong about anything, and that all the pains I have so humbly taken to verify my notions have only wasted my time!
>
> <cite>George Bernard Shaw</cite>

{% highlight html %}
> The longer I live, the more I realize that I am never wrong about anything, and that all the pains I have so humbly taken to verify my notions have only wasted my time!
>
> <cite>George Bernard Shaw</cite>
{% endhighlight %}

***



## Syntax Highlighter

{% highlight js %}
  $('.top').click(function () {
    $('html, body').stop().animate({ scrollTop: 0 }, 'slow', 'swing');
  });
  $(window).scroll(function () {
    if ($(this).scrollTop() > $(window).height()) {
      $('.top').addClass("top-active");
    } else {
      $('.top').removeClass("top-active");
    };
  });
{% endhighlight %}

***

## Images

<div class="gallery-box">
  <div class="gallery">
    <img src="/images/17.jpg">
    <img src="/images/07.jpg">
    <img src="/images/08.jpg">
    <img src="/images/22.jpg">
    <img src="/images/10.jpg">
    <img src="/images/21.jpg">
    <img src="/images/29.jpg">
    <img src="/images/30.jpg">
    <img src="/images/31.jpg">
  </div>
  <em>Gallery / <a href="https://unsplash.com/" target="_blank">Unsplash</a></em>
</div>

![]({{site.baseurl}}/images/140.jpg)
*Beautiful place*

{% highlight markdown %}
  ![]({{site.baseurl}}/images/140.jpg)
  *Beautiful place*
{% endhighlight %}

***

## Videos

<p><iframe src="https://www.youtube.com/embed/iWowJBRMtpc" frameborder="0" allowfullscreen></iframe></p>

{% highlight html %}
  <iframe src="https://www.youtube.com/embed/iWowJBRMtpc" frameborder="0" allowfullscreen></iframe>
{% endhighlight %}

***