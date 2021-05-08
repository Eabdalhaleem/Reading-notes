# Image
There are many reasons why you might 
want to add an image to a web page: you 
might want to include a logo, photograph, 
illustration, diagram, or chart.
As a website grows, keeping 
images in a separate folder 
helps you understand how the 
site is organized. Here you can 
see an example of the files for 
a website; all of the images are 
stored in a folder called images.

------
## Adding Images:
`<img>` 
To add an image into the page 
you need to use an `<img>`
element. This is an empty 
element (which means there is 
no closing tag). It must carry the 
following two attributes:
src
This tells the browser where 
it can find the image file. This 
will usually be a relative URL 
pointing to an image on your 
own site. 

**alt**
This provides a text description of the image which describes the image if you cannot see it.
**title**
You can also use the titleattribute with the `<img>` element 
to provide additional information 
about the image. Most browsers 
will display the content of this 
attribute in a tootip when the 
user hovers over the image
![img](https://cdo-curriculum.s3.amazonaws.com/media/uploads/img_tag.png)
----

## Height & Width of images
- height
This specifies the height of the image in pixels.
- width
This specifies the width of the image in pixels
![width](https://i.ytimg.com/vi/U1DKB4K4jX0/maxresdefault.jpg)
-----
## Where to Place Images in Your Code
1- before a paragraph The paragraph starts on a new line after the image.
2- inside the start of a paragraph The first row of text aligns with 
the bottom of the image.
3- in the middle of a paragraph The image is placed between the 
words of the paragraph that it appears in.

-----

**align** 
The align attribute was 
commonly used to indicate how 
the other parts of a page should 
flow around an image. It has 
been removed from HTML5


------
There are three **rules** to remember when you 
are creating **images** for your website which are 
summarized below. We go into greater detail 
on each topic over the next nine pages

* Save images in the right format
Websites mainly use images in jpeg, gif, or png format. If you choose the wrong image format then your image might not look as sharp as it should 
and can make the web page slower to load.

* Save images at the right size You should save the image at 
the same width and height it will appear on the website. If 
the image is smaller than the width or height that you have 
specified, the image can be distorted and stretched. If the 
image is larger than the width and height if you have specified, 
the image will take longer to display on the page.

* Use the correctresolution
Computer screens are made up 
of dots known as pixels. Images 
used on the web are also made 
up of tiny dots. Resolution refers 
to the number of dots per inch, 
and most computer screens only 
show web pages at 72 pixels 
per inch. So saving images at 
a higher resolution results in 
images that are larger than 
necessary and take longer to 
download

----

* The images you use on your website should be 
saved at the same width and height that you 
want them to appear on the page.

* When cropping images it is important not to 
lose valuable information. It is best to source 
images that are the correct shape if possible.

* Images created for the web should be saved at 
a resolution of 72 ppi. The higher the resolution 
of the image, the larger the size of the file

* Vector images differ from bitmap images and 
are resolution-independent. Vector images are 
commonly created in programs such as Adobe 
Illustrator.

* Animated GIFs show several frames of an 
image in sequence and therefore can be used to 
create simple animations.

* Transparency: Creating an image that is partially transparent (or "see-through") for the web involves 
selecting one of two formats:
- Transparent GIF
- PNG

--------

# HTML5: Figure and Figure Caption

`<figure>`
Images often come with 
captions. HTML5 has introduced 
a new `<figure> `element to 
contain images and their caption 
so that the two are associated. 
You can have more than one 
image inside the `<figure>`
element as long as they all share 
the same caption.
`<figcaption>`
The `<figcaption>` element has 
been added to HTML5 in order 
to allow web page authors to add 
a caption to an image.
Before these elements were 
created there was no way to 
associate an` <img>` element with 
its caption.
Older browsers that do not 
understand HTML5 elements 
simply ignore the new elements 
and display the content of them


-------

The `<img>` element is used to add images to a web page.
- You must always specify a src attribute to indicate the 
source of an image and an alt attribute to describe the 
content of an image.
- You should save images at the size you will be using 
them on the web page and in the appropriate format.
- Photographs are best saved as JPEGs; illustrations or 
logos that use flat colors are better saved as GIFs.


-------

# Colors


The color property allows you to specify the color of text inside 
an element. You can specify any color in CSS in one of three ways:
* rgb values
These express colors in terms of how much red, green and 
blue are used to make it up. For example: rgb(100,100,90)
* hex codes
These are six-digit codes that represent the amount of red, 
green and blue in a color, preceded by a pound or hash # sign.
 For example: #ee3e80
* color names
There are 147 predefined color names that are recognized 
by browsers. For example: DarkCyan

![color](https://make.wordpress.org/core/files/2021/02/wordpress-admin-color-palette-WP57.png)


---

# Background Color (background-color)

CSS treats each HTML element 
as if it appears in a box, and the 
background-color property 
sets the color of the background 
for that box.
You can specify your choice of 
background color in the same 
three ways you can specify 
foreground colors: RGB values, 
hex codes, and color names

------------

Every color on a computer screen is created by mixing amounts of red, 
green, and blue. To find the color you want, you can use a color picker.

----------

**RGB Values**
Values for red, green, and blue 
are expressed as numbers 
between 0 and 255. 
**rgb(102,205,170)**
This color is made up of the 
following values:
102 red
205 green
170 blue
 
- **Hex Codes**
Hex values represent values 
for red, green, and blue in 
hexadecimal code.
**#66cdaa**
The value of the red, 102, is 
expressed as 66 in hexadecimal 
code. The 205 of the green is 
expressed as cd and the 170 of 
the blue equates to aa.

- **Color Names**
Colors are represented by 
predefined names. However, 
they are very limited in number.
MediumAquaMarine
There are 147 color names 
supported by browsers (this 
color is MediumAquaMarine). 
Most consider this to be a 
limited color palette, and it is 
hard to remember the name for 
each of the colors so (apart from 
white and black) they are not 
commonly used

----
# Hsl, Hsla
The hsl color property has 
been introduced in CSS3 as an 
alternative way to specify colors. 
The value of the property starts 
with the letters hsl, followed 
by individual values inside 
parentheses for:
## hue
This is expressed as an angle 
(between 0 and 360 degrees).
saturation
This is expressed as a 
percentage.
## lightness
This is expressed as a 
percentage with 0% being white, 
50% being normal, and 100% 
being black.
The hsla color property allows 
you to specify color properties 
using hue, saturation, and 
lightness as above, and adds a 
fourth value which represents 
transparency (just like the rgba
property). The a stands for:
## alpha
This is expressed as a 
number between 0 and 1.0. 
For example, 0.5 represents 
50% transparency, and 0.75
represents 75% transparency.


--------

- color not only brings your site to life, but also helps 
convey the mood and evokes reactions.
- There are three ways to specify colors in CSS: 
RGB values, hex codes, and color names.
- Color pickers can help you find the color you want.
- It is important to ensure that there is enough contrast 
between any text and the background color (otherwise 
people will not be able to read your content).
- CSS3 has introduced an extra value for RGB colors to 
indicate opacity. It is known as RGBA.
- CSS3 also allows you to specify colors as HSL values, 
with an optional opacity value. It is known as HSLA.

-----

 ## Text


 The properties that allow you to control 
the appearance of text can be split into 
two groups:
● Those that directly affect the font and its appearance 
(including the typeface, whether it is regular, bold or italic, 
and the size of the text)
● Those that would have the same effect on text no matter 
what font you were using (including the color of text and 
the spacing between words and letters)

---------
# Typeface Terminology

* Serif 
Serif fonts have extra details on 
the ends of the main strokes of 
the letters. These details are 
known as serifs

* Sans-Serif
Sans-serif fonts have straight 
ends to letters, and therefore 
have a much cleaner design.

* Monospace
Every letter in a monospace (or 
fixed-width) font is the same 
width. (Non-monospace fonts 
have different widths.)

---------

When choosing 
a typeface, it is important to 
understand that a browser will usually 
only display it if it's installed on that 
user's computer.
Serif
Serif fonts have extra details on 
the end of the main strokes of 
the letters.
Sans-Serif
Sans-serif fonts have straight 
ends to letters and therefore 
have a much cleaner design

-----
# Specifying Typefaces

**The font-family** property 
allows you to specify the 
typeface that should be used for 
any text inside the element(s) to 
which a CSS rule applies.
The value of this property is the 
name of the typeface you want 
to use. 
The people who are visiting 
your site need the typeface you 
have specified installed on their 
computer inorder for it to be 
displayed.

 -------

 **The font-size** property enables 
you to specify a size for the 
font. There are several ways to 
specify the size of a font. The 
most common are:

## pixels
Pixels are commonly used 
because they allow web 
designers very precise control 
over how much space their text 
takes up. The number of pixels is 
followed by the letters px.

## percentages 
The default size of text in 
browsers is 16px. So a size of 
75% would be the equivalent of 
12px, and 200% would be 32px**

-------

## font-face

@font-face allows you to use 
a font, even if it is not installed 
on the computer of the person 
browsing, by allowing you to 
specify a path to a copy of the 
font, which will be downloaded if 
it is not on the user's machine.

----------

## font-family
This specifies the name of the 
font. This name can then be used 
as a value of the font-family
property in the rest of the style 
sheet (as shown in the rule for 
the `<h1>` and `<h2>` elements).

## src
This specifies the path to the 
font. In order for this technique 
to work in all browsers, you will 
probably need to specify paths 
to a few different versions of the 
font, as shown on the next page.

## format
This specifies the format that the 
font is supplied in. (It's discussed 
in detail on the next page.)

------

# font-weight

The font-weight property 
allows you to create bold text. 
There are two values that this 
property commonly takes:

## normal
This causes text to appear at a 
normal weight.
## **bold**
This causes text to appear bold.
In this example, you can see 
that the element whose class
attribute has a value of credits
has been bolded

--------
# font-style

If you want to create *ilatic* text, you can use the font-style
property. There are three values this property can take:

**normal** 
This causes text to appear in a 
normal style (as opposed to italic 
or oblique).

*italic*
This causes text to appear italic.

**oblique**
This causes text to appear 
oblique 

-------
# The text-transform 
property 
is used to change the case of 
text giving it one of the following 
values:

- *uppercase* This causes the text to appear 
uppercase.

- *lowercase*
This causes the text to appear 
lowercase.

- *capitalize*
This causes the first letter of 
each word to appear capitalized

------------

## The text-decoration
 property 
allows you to specify the 
following values:

**none**
This removes any decoration 
already applied to the text.

**underline**
This adds a line underneath the 
text.

**overline**
This adds a line over the top of 
the text.

**line-through**
This adds a line through words

**blink**
This animates the text to make it 
flash on and off (however this is 
generally frowned upon, as it is 
considered rather annoying).
In this example, the credits hav

---------

# Alignment
## text-align 
The text-align property allows 
you to control the alignment of 
text. The property can take one 
of four values:

## left
This indicates that the text 
should be left-aligned.

## right
This indicates that the text 
should be right-aligned.

## center
This allows you to center text.

## justify
This indicates that every line in 
a paragraph, except the last line, 
should be set to take up the full 
width of the containing box

-----
# Vertical Alignment
## vertical-align

The vertical-align property is 
a common source of confusion. 
It is not intended to allow you to 
vertically align text in the middle 
of block level elements such as 
<p> and <div>, although it does 
have this effect when used with 
table cells (the <td> and <th>
elements).

# Indenting Text
## text-indent

The text-indent property 
allows you to indent the first 
line of text within an element. 
The amount you want the line 
indented by can be specified in 
a number of ways but is usually 
given in pixels or ems

-----

#  Drop Shadow
## text-shadow

The text-shadow property has 
become commonly used despite 
lacking support in all browsers. 
It is used to create a drop 
shadow, which is a dark version 
of the word just behind it and 
slightly offset. It can also be used 
to create an embossed effect by 
adding a shadow that is slightly 
lighter than the text.
The value of this property is 
quite complicated because it can 
take three lengths and a color for 
the drop shadow.


-----

# First Letter or Line
## :first-letter, :first-line

You can specify different values 
for the first letter or first line of 
text inside an element using
:first-letter and 
:first-line. 
Technically these are not 
properties. They are known as 
pseudo-elements.
You specify the pseudo-element 
at the end of the selector, and 
then specify the declarations as 
you would normally for any other 
element

-------

# Styling Links
## :link, :visited

Browsers tend to show links 
in blue with an underline by 
default, and they will change 
the color of links that have been 
visited to help users know which 
pages they have been to.


------

# :link
This allows you to set styles 
for links that have not yet been 
visited.

# :visited
This allows you to set styles for 
links that have been clicked on. 
They are commonly used to 
control colors of the links and 
also whether they are to appear 
underlined or not

-------

# Responding to Users
## :hover, :active, :focus

There are three pseudo-classes 
that allow you to change the 
appearance of elements when a 
user is interacting with them.

## :hover
This is applied when a user 
hovers over an element with a 
pointing device such as a mouse. 
This has commonly been used 
to change the appearance of 
links and buttons when a user 
places their cursor over them

# :active
This is applied when an element 
is being activated by a user; for 
example, when a button is being 
pressed or a link being clicked. 
Sometimes this is used to make 
a button or link feel more like it 
is being pressed by changing the 
style or position of the element 
slightly.

# :focus
This is applied when an element 
has focus. Any element that 
you can interact with, such as a 
link you can click on or any form 
control can have focus.

------

![text](https://cdn.educba.com/academy/wp-content/uploads/2019/08/CSS-Text-Formatting-Properties2.png)


* There are properties to control the choice of font, size, 
weight, style, and spacing.

* There is a limited choice of fonts that you can assume 
most people will have installed.

* If you want to use a wider range of typefaces there are 
several options, but you need to have the right license 
to use them.

* You can control the space between lines of text, 
individual letters, and words. Text can also be aligned 
to the left, right, center, or justified. It can also be 
indented.

* You can use pseudo-classes to change the style of an 
element when a user hovers over or clicks on text, or 
when they have visited a link

--------

## JPEG vs PNG vs GIF

TL;DR
Use **JPEG** format for all images that contain a natural scene or photograph where variation in colour and intensity is smooth. Use PNG format for any image that needs transparency or for images with text & objects with sharp contrast edges like logos. Use GIF format for images that contain animations.
Compression
Almost all forms of data that we see on the internet — text, image, video etc. — are compressed to reduce the size of data and ensure faster transmission. Choosing the correct format and compression is a major factor that determines image size.


**PNG** is a lossless image format using DEFLATE compression. No data is lost during compression and no compression artefacts are introduced in the image. For this reason, a PNG image would retain higher quality than an image than JPEG and would look a lot sharper, it would also occupy more space on the disk. This makes it unsuitable for storing or transferring high-resolution digital photographs but a great choice for images with text, logos and shapes with sharp edges.

**GIF** is also a lossless image format that uses LZW compression algorithm. It was favoured over PNG for simple graphics in websites in its early days because the support of PNG was still growing. Given that PNG is now supported across all major devices and that PNG compression is about 5–25% better than GIF compression, GIF images are now mainly used only if the image contains animations.

--------

**JPEG** images don’t support transparency and are hence not usable for such cases.

**PNG** images support transparency in two ways — inserting an alpha channel that allows partial transparency or by declaring a single colour as transparent (index transparency). Partial transparency makes the edges blend smoothly into the background. PNG8 images (discussed in the “Colours” section below) can support only index transparency whereas PNG24 images can support alpha channel transparency.

**GIF** images support transparency by declaring a single colour in the colour palette as transparent (index transparency). Because of absence of partial transparency, the edges (specially rounded or too-detailed edges) get a poor jagged effect. Though this can be solved to some extent using dithering, with improved PNG support, GIF is unsuitable for images with transparent backgrounds.

---------------
## Colours
There is a significant difference in the number of colours that can be supported by these 3 formats.
**JPEG** images can support around 16 million colours. This is what makes them suitable for storing images of natural scenes.

**PNG** images mainly have two modes — PNG8 and PNG24. PNG8 can support upto 256 colours whereas PNG24 can handle upto 16 million colours like a JPEG image. Use PNG8 for simple shapes with fewer colours and PNG24 for high quality, complex logos and shapes with rounded corners on a transparent background.

**GIF** images are limited to 256 colours. If index transparency is used, then one of these 256 colours is assigned as transparent and the remaining 255 are used for other colours.

-------

**Animation**
Animation, in this case, refers to any change or movement in the image. It doesn’t necessarily have to have frame rates like an animated video, but essentially a part or the entire image changes with time.
Of these 3 formats, only **GIF** supports animation. This capability makes GIF format suitable for delivering engaging ads and banners. Of late, with the advent of companies Tumblr, 9Gag, Giphy etc. the use of GIF format for memes has picked up











