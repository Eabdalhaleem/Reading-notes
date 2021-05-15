# Images
Controlling the size and alignment of your images using CSS keeps rules that 
affect the presentation of your page in the CSS and out of the HTML markup.
You can also achieve several interesting effects using background images. In this chapter you will learn how to:

* Specify the size and alignment of an image using
* Add background images to boxes
* Create image rollovers in CSS.

-------


![ss](https://www.lambdatest.com/blog/wp-content/uploads/2021/05/how-to-make-a-responsive-background-image-using-css.jpg)


## Controlling sizes of images in CSS:

You can control the size of an image using the width and 
height properties in CSS, just like you can for any other box. 
Specifying image sizes helps pages to load more smoothly 
because the HTML and CSS code will often load before the 
images, and telling the browser how much space to leave for an 
image allows it to render the rest of the page without waiting for 
the image to download.You might think that your site 
is likely to have images of all different sizes, but a lot of sites 
use the same sized image across many of their pages. 

-------

First you need to determine the sizes of images that will be used 
commonly throughout the site, then give each size a name.
For example:
* small
* medium
* large
Where the `<img>` elements appear in the HTML, rather 
than using width and height attributes you can use these 
names as values for the class attribute. 
In the CSS, you add selectors for each of the class names, then 
use the CSS width and height properties to control the image dimensions.

-------------

## AligNing images using CSS

* The float property is added to the class that was created to 
represent the size of the image .

* New classes are created with names such as align-left or 
align-right to align the images to the left or right of the page. 
These class names are used in addition to classes that indicate 
the size of the image.

---------

## Centering images using CSS

By default, images are inline elements. This means that they 
flow within the surrounding text. In order to center an image, it 
should be turned into a blocklevel element using the display
property with a value of block. 
Once it has been made into a block-level element, there are 
two common ways in which you can horizontally center an image:

* On the containing element, you can use the text-align
property with a value of center.

* On the image itself, you can use the use the margin property 
and set the values of the left and right margins to auto.
You can specify class names that allow any element to be 
centered, in the same way that you can for the dimensions or 
alignment of images

-----------

Background Images`background-image`

The background-image property allows you to place 
an image behind any HTML element. This could be the entire 
page or just part of the page. By default, a background image will 
repeat to fill the entire box.The path to the image follows 
the letters url, and it is put inside parentheses and quotes

----------

## Repeating Images
`background-attachment`
`background-repeat`

The background-repeat
property can have four values:

**repeat**
The background image is 
repeated both horizontally and 
vertically (the default way it 
is shown if the backgroundrepeat property isn't used).

**repeat-x**
The image is repeated 
horizontally only (as shown in 
the first example on the left).

**repeat-y**
The image is repeated vertically 
only.

**no-repeat**
The image is only shown once.
The background-attachment 
property specifies whether a 
background image should stay in 
one position or move as the user 
scrolls up and down the page. It 
can have one of two values:

**fixed**
The background image stays in 
the same position on the page.

**scroll**
The background image moves 
up and down as the user scrolls 
up and down the page.

-----------

## Background Position

When an image is not being repeated, you can use the 
background-position property to specify where in the 
browser window the background image should be placed. 
This property usually has a pair of values. The first represents 
the horizontal position and the second represents the vertical

---------

## shorthand (background)

The background property acts like a shorthand for all of the other background properties 
you have just seen, and also the background-color property.
The properties must be specified in the following order, but you 
can miss any value if you do not want to specify it.
* background-color
* background-image
* background-repeat
* background-attachment
* background-position
CSS3 will also support the use of multiple background images 
by repeating the backgroundshorthand. Because few 
browsers supported this property at the time of writing, it 
was not commonly used

---------

## Image Rollovers & Sprites

Using CSS, it is possible to create a link or button that changes to a 
second style when a user moves their mouse over it (known as a 
rollover) and a third style when they click on it.

This is achieved by setting a background image for the link or 
button that has three different styles of the same button (but 
only allows enough space to show one of them at a time). 
You can see the image we are using in this example on the 
right. It actually features two buttons on the one image.
When the user moves their mouse over the element, or 
clicks on it, the position of the background image is moved to 
show the relevant image.When a single image is used 
for several different parts of an interface, it is known as a sprite. 
You can add the logo and other interface elements, as well as 
buttons to the image.The advantage of using sprites is 
that the web browser only needs to request one image rather than 
many images, which can make the web page load faster

------

## CSS3: Gradients (background-image)

CSS3 is going to introduce the 
ability to specify a gradient for 
the background of a box. The 
gradient is created using the 
background-image property 
and, at the time of writing, 
different browsers required a 
different syntax.
Since it is not supported by all 
browsers, it is possible to specify 
a background image for the box 
first (which would represent the 
gradient) and then provide the 
CSS alternatives for browsers 
that support gradients.

-------  

## Contrast of background images

If you want to overlay text on a background image, the image must be low 
contrast in order for the text to be legible

**High Contrast** 
A high contrast background 
image makes the text difficult 
to read.

**Low Contrast**
A low contrast background 
image makes 
the text easier to read.

 **Screen**
A screen added to a high 
contrast image makes the text easier to read.

----------

* You can specify the dimensions of images using CSS. 

This is very helpful when you use the same sized 
images on several pages of your site.

* Images can be aligned both horizontally and vertically 
using CSS.

* You can use a background image behind the box 
created by any element on a page. 

* Background images can appear just once or be 
repeated across the background of the box.

* You can create image rollover effects by moving the 
background position of an image.

* To reduce the number of images your browser has to 
load, you can create image sprites.



![image](https://img.webnots.com/2017/03/CSS-Image-Overlay-Effects.png)

---------

## Practical Information

To wrap up the book we are going to look at some practical information that will 
help you launch a successful site.
There are entire books written about each of the topics covered in this chapter but I will introduce you to the key themes that each subject deals with and give you pointers for what you need to be considering. You will see:
* The basics of search engine optimization
* Using analytics to understand how people are using your 
site after it has launched
* Putting your site on the web

----

## Search Engine Optimization (SEO)

SEO is a huge topic and several books have been written on the subject. 
The following pages will help you understand the key concepts so you can 
improve your website's visibility on search engines

## The Basics
Search engine optimization (or SEO) is the practice of trying 
to help your site appear nearer the top of search engine results 
when people look for the topics that your website covers.
At the heart of SEO is the idea of working out which terms people 
are likely to enter into a search engine to find your site and then 
using these terms in the right places on your site to increase 
the chances that search engines will show a link to your site in 
their results

-----

## On-Page Techniques

On-page techniques are the methods you can use on your 
web pages to improve their rating in search engines.
The main component of this is looking at keywords that people 
are likely to enter into a search engine if they wanted to find 
your site, and then including these in the text and HTML code 
for your site in order to help the search engines know that your 
site covers these topics

----

## Off-Page Techniques
Getting other sites to link to you is just as important as on-page 
techniques. Search engines help determine how to rank your 
site by looking at the number of other sites that link to yours.
They are particularly interested in sites whose content is related 
to yours. For example, if you were running a website that 
sold fish bait, then a link from a hairdresser is not likely to be 
considered as relevant as one from an angling community.

----------

# On-Page SEO

In every page of your website there are seven key places where keywords 
(the words people might search on to find your site) can appear in order 
to improve its findability.

* **Page Title**
The page title appears at the top 
of the browser window or on the 
tab of a browser. It is specified in 
the `<title>` element which lives 
inside the `<head>` element.

* **URL / Web Address**
The name of the file is part of 
the URL. Where possible, use 
keywords in the file name.

* **Headings**
If the keywords are in a heading 
`<hn> `element then a search 
engine will know that this page is 
all about that subject and give it 
greater weight than other text.

* **Text**
Where possible, it helps to 
repeat the keywords in the main 
body of the text at least 2-3 
times. Do not, however, over-use 
these terms, because the text 
must be easy for a human to read

* **Link Text**
Use keywords in the text that 
create links between pages 
(rather than using generic 
expressions such as "click here").
* **Image Alt Text**
Search engines rely on you 
providing accurate descriptions 
of images in the alt text. This 
will also help your images show 
up in the results of image-based 
searches.
* **Page Descriptions**
The description also lives inside 
the` <head>` element and is 
specified using a `<meta>` tag. 
It should be a sentence that 
describes the content of the 
page. (These are not shown in 
the browser window but they 
may be displayed in the results 
pages of search engines.)

----------

## How to Identify Keywords and Phrases

Determining which keywords to use on your site can be one of the 
hardest tasks when you start to think about SEO. Here are six steps that 
will help you identify the right keywords and phrases for your site.

* **Brainstorm**
List down the words that someone might type into 
Google to find your site. Be sure to include the various topics, 
products or services your site is about.
It often helps to ask other people what words they would use to 
find your site because people less familiar with a topic might 
use different terms than you. (In particular, they are less likely to 
use industry-specific jargon.)

* **Organize**
Group the keywords into separate lists for the different 
sections or categories of your website.
For example, if your website was a pet shop you might have 
different categories for different animals (such as dogs, cats and 
rabbits)

* **Research**
There are several tools that let you enter your keywords and 
then they will suggest additional keywords you might like to 
consider, such as:
**adwords.google.co.uk/**

select/KeywordToolExternal
(When using this tool, select the 
"exact match" option rather than 
"broad match.")
**www.wordtracker.com**
**www.keyworddiscovery.com**

* **Compare**
It is very unlikely that your site will appear at the top of 
the search results for every keyword. This is especially true 
for topics where there is a lot of competition. The more sites 
out there that have already been optimized for a given keyword, 
the harder it will be for you to rise up the search results when 
people search on that term.


* **Refine**
Now you need to pick which keywords you will focus on. 
These should always be the ones that are most relevant to each 
section of your site.If there is a phrase that is very 
relevant but you find there is a lot of competition, you should 
still use it. To improve the chances of your site being found 
you can look at whether there are other words that could be 
incorporated into a phrase. For example, if the information or service you offer on your website 
is location specific, then you will often find that incorporating 
your location into your keyword list will help people find you.

* **Map**
Now that you have a refined list of keywords, you know which 
have the most competition, and which ones are most relevant, 
it is time to start picking which keywords you will use for each 
page.Pick 3-5 keywords or phrases that map to each page of your 
website and use these as the keywords for each page.

-------

## Analytics: Learning about your Visitors

As soon as people start coming to your site, you can start analyzing 
how they found it, what they were looking at and at what point they are 
leaving. One of the best tools for doing this is a free service offered by 
Google called Google Analytics.

* **Signing Up**
The Google Analytics service 
relies on you signing up for an 
account at:
www.google.com/analytics
The site will give you a piece of 
tracking code which you need to 
put on every page of your site.

* **How it Works**
Every time someone loads a 
page of your site, the tracking 
code sends data to the Google 
servers where it is stored. 
Google then provides a webbased interface that allows you 
to see how visitors use your site

* **The Tracking Code**
A tracking code is provided 
by Google Analytics for each 
website you are tracking. It 
should appear just before the 
closing `</head>` tag. The code 
does not alter the appearance of 
your web pages

-------------

## How Many People Are Coming to Your Site? 
The overview page gives you a snapshot of the key information you are 
likely to want to know. In particular, it tells you how many people are 
coming to your site

**Visits**
This is the number of times 
people have come to your site. If 
someone is inactive on your site 
for 30 minutes and then looks at 
another page on your site, it will 
be counted as a new visit

**Unique Visits**
This is the total number of 
people who have visited your site 
over the specified period. The 
number of unique visits will be 
lower than the number of visits 
if people have been returning to 
your site more than once in the 
defined period

**Page Views**
The total number of pages all 
visitors have viewed on your site.

**Pages per Visit**
The average number of pages 
each visitor has looked at on 
your site per visit.

**Average Time on Site**
The average amount of time 
each user has spent on the site 
per visit.

**Date Selector**
Using the date selector in the top 
right hand corner of the site, you 
can change the period of time 
the reports display. When you 
log in, this is usually set to the 
last month, but you can change 
it to report on a specific time 
period.

**Export**
The export link just above the 
title that says "visitors overview" 
allows you to export the 
statistics on this page for other 
applications such as Excel

--------

## What Are Your Visitors Looking At?

The content link on the left-hand side allows 
you to learn more about what the visitors are 
looking at when they come to your site.
What Are Your Visitors Looking At?

**Pages**
This tells you which pages your 
visitors are looking at the most 
and also which pages they are 
spending the most time on

**Landing Pages**
These are the pages that people 
arrive on when first visiting your 
site. This can be particularly 
helpful because you may find 
people are not always coming 
into your site via the homepage.

**Top Exit Pages**
This shows which pages people 
most commonly leave from. If 
a lot of people are leaving from 
the same page then you might 
consider changing that page or 
improving it

**Bounce Rate**
This shows the number of people 
who left on the same page that 
they arrived on. A high bounce 
rate suggests that the content is 
not what they were looking for or 
that the page did not sufficiently 
encourage them to look around 
the rest of the site. What counts 
as a bounce:
* Clicked a link to another site
* Clicked on an advertisement
* Entered a new URL
* Used the "back" button
* Closed the browse


-----------------

## Where Are Your Visitors Coming From?
The traffic sources link on the left hand side 
allows you to learn where your visitors are 
coming from.

**Referrers**
This shows the sites that have 
linked to you and the number 
of people who have come via 
those sites. If a site sends a lot 
of traffic to you, get in touch and 
try to work together to ensure 
that traffic keeps flowing. You 
could also try to find similar 
sites and ask them to link to you

**Direct**
This shows which page a user 
arrived on if they did not come 
via a link on another site. They 
might have typed the URL into 
their browser, used a browser 
bookmark, or clicked a link in an 
email, PDF, or Word document

**Search Terms**
This shows the terms users 
entered into a search engine 
to find your site. This can help 
you learn how visitors describe 
what they're looking for (which is 
often different to how someone 
might describe their own site). 
This can help you fine-tune your 
content and your SEO keywords

**Advanced Features**
We have only scratched the 
surface of what you can find 
out about your visitors from 
Google Analytics. Their help 
files tell you many more of the 
advanced features.
 If you run an online shop, it is well worth 
looking at their e-commerce 
tracking, which adds information 
about products sold, average 
basket size and much more. 
You can also set up goals where 
you specify the paths you want 
people to take, and then see how 
far they get through those paths, 
which is especially useful when 
gathering data from users

---------

## Domain Names & Hosting
In order to put your site on the web you will 
need a domain name and web hosting

**DOMAIN NAMES** 
Your domain name is your web 
address `(e.g. google.com or bbc.
co.uk)`. There are many websites 
that allow you to register domain 
names. Usually you will have to 
pay an annual fee to keep that 
domain name.

**WEB Hosting**
So that other people can see 
your site, you will need to upload 
it to a web server. Web servers 
are special computers that are 
constantly connected to the 
Internet. They are specially set 
up to serve web pages when 
they are requested

**Disk space**
This refers to the total size of all 
of the files that make up your site 
(all of the HTML and CSS files, 
images and scripts).

**Bandwidth**
This is the amount of data the 
hosting company will send to 
your site's visitors. If you imagine 
10 people looked at every page 
on your site, then it would be 
the equivalent to 10 times the 
amount of disk space you use.

**Backups**
Check whether the hosting 
company performs backups on 
your site (and how often). Some 
only create backups so that 
they can restore your website in 
the event of a server breaking. 
Others allow access to backups 
(which can be helpful if you 
accidentally break the site when 
updating it)

----------

## FTP & Third Party Tools

To transfer your code and images from your 
computer to your hosting company, you use 
something known as File Transfer Protocol

There are a wide variety of sites that offer 
services commonly created by web developers 
(to save you having to build them yourself).

Here is a list of some popular 
third party tools:
**Blogs**
`wordpress.com`
`tumblr.com`
`posterous.com`
**E-commerce**
`shopify.com`
`bigcartel.com`
`go.magento.com`
**Email newsletters**
`campaignmonitor.com`
`mailchimp.com`
**Social networking** 
**sharing buttons**
`addthis.com`
`addtoany.com`

--------

* Search engine optimization helps visitors find your 
sites when using search engines.

* Analytics tools such as Google Analytics allow you to 
see how many people visit your site, how they find it, 
and what they do when they get there.

* To put your site on the web, you will need to obtain a 
domain name and web hosting.

* FTP programs allow you to transfer files from your 
local computer to your web server.

* Many companies provide platforms for blogging, email 
newsletters, e-commerce and other popular website 
tools (to save you writing them from scratch)

--------

## Video and Audio APIs

HTML5 comes with elements for embedding rich media in documents — `<video>` and <audio> — which in turn come with their own APIs for controlling playback, seeking, etc. This article shows you how to do common tasks such as creating custom playback controls

**HTML5 video and audio**
The `<video>` and `<audio>` elements allow us to embed video and audio into web pages. As we showed in Video and audio content

You can review what all the HTML features do in the article linked above; for our purposes here, the most interesting attribute is controls, which enables the default set of playback controls. If you don't specify this,

**The HTMLMediaElement API**
Part of the HTML5 spec, the HTMLMediaElement API provides features to allow you to control video and audio players programmatically — for example HTMLMediaElement.play(), HTMLMediaElement.pause(), etc. This interface is available to both `<audio>` and `<video>` elements, as the features you'll want to implement are nearly identical. Let's go through an example, adding features as we go.

**Implementing the JavaScript**
We've got a fairly complete HTML and CSS interface already; now we just need to wire up all the buttons to get the controls working.

Here we are creating constants to hold references to all the objects we want to manipulate. We have three groups:

The `<video>` element, and the controls bar.
The play/pause, stop, rewind, and fast forward buttons.
The outer timer wrapper `<div>`, the digital timer readout `<span>`, and the inner` <div> `that gets wider as the time elapses.

I think we've taught you enough in this article. The HTMLMediaElement API makes a wealth of functionality available for creating simple video and audio players, and that's only the tip of the iceberg. See the "See also" section below for links to more complex and interesting functionality.

Here are some suggestions for ways you could enhance the existing example we've built up:

The time display currently breaks if the video is an hour long or more (well, it won't display hours; just minutes and seconds). Can you figure out how to change the example to make it display hours?

Because `<audio>` elements have the same HTMLMediaElement functionality available to them, you could easily get this player to work for an `<audio>` element too. Try doing so.

Can you work out a way to turn the timer inner `<div>` element into a true seek bar/scrobbler — i.e., when you click somewhere on the bar, it jumps to that relative position in the video playback? As a hint, you can find out the X and Y values of the element's left/right and top/bottom sides via the getBoundingClientRect() method, and you can find the coordinates of a mouse click via the event object of the click event, called on the Document object.

-----------------

Flash is a very popular technology used 
to add animations, video, and audio to 
websites. This chapter begins by looking 
at how to use it in your web pages.

We then focus on how to add video and audio to your site, 
using either the new HTML5 `<video>` and `<audio> `elements 
or a hosted service (such as YouTube or SoundCloud). In this 
chapter you will learn:

* How to use Flash in your web pages
* How to use HTML5 `<video>` and `<audio>` elements
* When to host your own video and audio and when to use a 
service such as YouTub

-------

**How Flash Works**

Since the late 1990s, Flash has been a very 
popular tool for creating animations, and later 
for playing audio and video in websites

Whether you are creating an 
animation or a media player in 
Flash, the files you put on your 
website are referred to as Flash 
movies. 
If you want to create your 
own Flash movie, you need to 
purchase the Flash authoring 
environment from Adobe.

When you create a Flash file in 
the Flash authoring environment, 
it is saved with the .fla file 
extension. In order to use this file 
on a web page it has to be saved 
in a different format known 
as SWF. (It has the .swf file 
extension.

To view Flash, browsers need 
to use a plugin (an extra piece 
of software that runs in the 
browser) called the Flash Player. 
Statistics commonly indicate 
that 98% of browsers on 
desktop computers have the 
Flash plugin installed. (The 
percentage of mobiles and 
tablets with it is much less.

-------

**Use of Flash**

Since 2005, a number of factors have meant 
that fewer websites are written in Flash or even 
use elements of Flash in their pages

--------

## Timeline:Flash, VidEo & Audio

Web technologies change quickly. Here you 
can see some of the changes in how animation, 
video, and audio are created on the web.

