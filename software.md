---
layout: page
title: Software Setup
permalink: /software/
modified: 2013-05-31
category: articles
# image:
#   feature: so-simple-sample-image-1.jpg
#   credit: Michael Rose
#   creditlink: http://mademistakes.com
comments: true
share: true
---

These are the steps necessary to get your Raspberry Pis talking to each other on
a network using MPI.

### Requirements

- Raspberry Pis running the Raspbian distribution
- A network router or switch to connect the Pis to

### Installation Steps

1. The first step is to power up each Pi and get Rasbian installed on the
   sdcard. Follow the [NOOBS Setup Guide](http://www.raspberrypi.org/help/noobs-setup/)
   for instructions.

2. Once you have Raspian running on each Pi you'll need to login to it either
   directly with a keyboard, mouse, and monitor or remotely over ssh.


# Heading 1

## Heading 2

### Heading 3

#### Heading 4

##### Heading 5

###### Heading 6

### Body text

Lorem ipsum dolor sit amet, test link adipiscing elit. **This is strong**.
Nullam dignissim convallis est. Quisque aliquam.

![Smithsonian Image]({{ site.url }}/images/3953273590_704e3899d5_m.jpg)
{: .pull-right}

*This is emphasized*. Donec faucibus. Nunc iaculis suscipit dui. 53 = 125. Water
is H<sub>2</sub>O. Nam sit amet sem. Aliquam libero nisi, imperdiet at,
tincidunt nec, gravida vehicula, nisl. The New York Times <cite>(That’s a
citation)</cite>. <u>Underline</u>. Maecenas ornare tortor. Donec sed tellus
eget sapien fringilla nonummy. Mauris a ante. Suspendisse quam sem, consequat
at, commodo vitae, feugiat in, nunc. Morbi imperdiet augue quis tellus.

HTML and <abbr title="cascading stylesheets">CSS<abbr> are our tools. Mauris a
ante. Suspendisse quam sem, consequat at, commodo vitae, feugiat in, nunc. Morbi
imperdiet augue quis tellus. Praesent mattis, massa quis luctus fermentum,
turpis mi volutpat justo, eu volutpat enim diam eget metus.

### Blockquotes

> Lorem ipsum dolor sit amet, test link adipiscing elit. Nullam dignissim convallis est. Quisque aliquam.

## List Types

### Ordered Lists

1. Item one
   1. sub item one
   2. sub item two
   3. sub item three
2. Item two

### Unordered Lists

* Item one
* Item two
* Item three

## Tables

| Header1 | Header2 | Header3 |
|:--------|:-------:|--------:|
| cell1   | cell2   | cell3   |
| cell4   | cell5   | cell6   |
|----
| cell1   | cell2   | cell3   |
| cell4   | cell5   | cell6   |
|=====
| Foot1   | Foot2   | Foot3
{: rules="groups"}

## Code Snippets

Syntax highlighting via Pygments

{% highlight css %}
#container {
  float: left;
  margin: 0 -240px 0 0;
  width: 100%;
}
{% endhighlight %}

Non Pygments code example

    <div id="awesome">
        <p>This is great isn't it?</p>
    </div>

## Buttons

Make any link standout more when applying the `.btn` class.

<div markdown="0"><a href="#" class="btn">This is a button</a></div>
