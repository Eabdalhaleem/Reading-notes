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
<img> 
To add an image into the page 
you need to use an <img>
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
You can also use the titleattribute with the <img> element 
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

------
There are three **rules to remember when you 
are creating images** for your website which are 
summarized below. We go into greater detail 
on each topic over the next nine pages

- Save images in the right format
Websites mainly use images in jpeg, gif, or png format. If you choose the wrong image format then your image might not look as sharp as it should 
and can make the web page slower to load.

- Save images at the right size You should save the image at 
the same width and height it will appear on the website. If 
the image is smaller than the width or height that you have 
specified, the image can be distorted and stretched. If the 
image is larger than the width and height if you have specified, 
the image will take longer to display on the page.

----
The <img> element is used to add images to a web page.
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
- rgb values
These express colors in terms of how much red, green and 
blue are used to make it up. For example: rgb(100,100,90)
- hex codes
These are six-digit codes that represent the amount of red, 
green and blue in a color, preceded by a pound or hash # sign.
 For example: #ee3e80
- color names
There are 147 predefined color names that are recognized 
by browsers. For example: DarkCyan

---

RGB Values
Values for red, green, and blue 
are expressed as numbers 
between 0 and 255. 
rgb(102,205,170)
This color is made up of the 
following values:
102 red
205 green
170 blue
- Hex Codes
Hex values represent values 
for red, green, and blue in 
hexadecimal code.
#66cdaa
The value of the red, 102, is 
expressed as 66 in hexadecimal 
code. The 205 of the green is 
expressed as cd and the 170 of 
the blue equates to aa.
- Color Names
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
olor not only brings your site to life, but also helps 
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
computer in
 -------

 **The font-size property** enables 
you to specify a size for the 
font. There are several ways to 
specify the size of a font. The 
most common are:
pixels
Pixels are commonly used 
because they allow web 
designers very precise control 
over how much space their text 
takes up. The number of pixels is 
followed by the letters px.
percentagesThe default size of text in 
browsers is 16px. So a size of 
75% would be the equivalent of 
12px, and 200% would be 32px**

-------
If you want to create italic text, you can use the font-style
property. There are three values this property can take:
normal This causes text to appear in a 
normal style (as opposed to italic 
or oblique).
italic
This causes text to appear italic.
oblique This causes text to appear 
oblique 

-------
The text-transform property 
is used to change the case of 
text giving it one of the following 
values:
uppercase
This causes the text to appear 
uppercase.
lowercase
This causes the text to appear 
lowercase.
capitalize
This causes the first letter of 
each word to appear capitalized

------------

The text-decoration property 
allows you to specify the 
following values:
none
This removes any decoration 
already applied to the text.
underline
This adds a line underneath the 
text.
overline
This adds a line over the top of 
the text.
line-through
This adds a line through words

---------
