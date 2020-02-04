# Frontend Mod 0 Capstone - Day 2 Exercises

## Exercises on Lists and Links

1. There are three types of lists in HTML: ordered lists, unordered lists and definition lists. They each have unique use cases.
    1. *Ordered lists* are used to describe information that only makes sense when displayed in a specific order. Examples might include recipes or driving directions. The `<ol></ol>` tags are used to denote an ordered list, and the individual items are displayed with the `<li></li>` tags.
    2. *Unordered lists* are used to describe information that does not necessarily need to be displayed in a specific order to make sense. Examples include a list of ingredients, or cities in a country. The `<ul></ul>` tags are used to show an unordered list, and the individual items in the list should be surrounded by `<li></li>` tags.
    3. *Definition lists* are used when stating the meaning of terms used in a body of work. An example is a glossary. Definition lists are surrounded by `<dl></dl>` tags. Each new term in the list is marked with `<dt></dt>` tags, and each term's definition is marked with `<dd></dd>` tags.
2. To link to another website, you use the *anchor* element. The tags used to display an anchor are `<a></a>`. To specify the url of the page to link to, the `href` attribute is used. For example, the HTML to link to twitter might look like this: `<a href="https://www.twitter.com">an addicting website</a>`.
3. To open a linked page in a new window, the `target` attribute should be given a value of `"_blank"`. For example, the html for a link to Reddit that opens in a new window would look like: `<a href="https://www.reddit.com" target="_blank">another addicting site</a>`.
4. To link to a specific part of the current page, you first need to make sure that the tag you want to link to has an `id` attribute. In the `href` attribute of the anchor elemement, you need to use that element's `id`, prepended by an `#` sign (I think that's called an octothorpe. What a cool name!). For example, to link to the introduction section of a page, there would need to be a tag like `<h2 id="introduction">The Introduction</h2>`, and then the link to go to that header would be `<a href="#introduction">Go to the Introduction</a>`.

## Exercises on CSS, Color, and Text
1. The purpose of CSS is to add style to an html document. This includes editing the colors, layout, and font of a webpage.
2. CSS stands for *cascading style sheets*. The word *cascading* is meant to indicate that general style rules can be defined, and will be inherited by the elements on a page, unless more specific rules are defined that apply to those elements.
3. A CSS rule consists of a *selector*, which specifies which html elements on a page the rule applies to, and a *declaration*, which defines how those elements should be styled. The declaration consist of a list of *properties* and *values*. Properties specify the characteristics of the selected elements that the rule applies to, and values define how these properties are changed by the rule. For example, we can make every level 1 header red with a blue background using this rule:
   ```css
    h1 {
      color: red;
      background: blue;
    }
   ```
   Here ```h1``` is the selector, the part enclosed in curly braces is the declaration, `color` and `background` are the properties, and `red` and `blue` are the values.
4. You link a css stylesheet to your html document by including a *link* element in the head of the html file. The link element consists of a single ``<link />`` tag that has three attributes:
   1. The `href` attribute must give a path to the linked stylesheet.
   2. The `type` attribute should be set to `text/css`.
   3. The `rel` attribute should be set to `stylesheet`.
   For example, the following head of an html documents links to a sylesheet called ```fonts.css``` in the ```css``` directory:
   ```HTML
    <head>
      ...
      <link href="css/fonts.css" type="text/css" rel="stylesheet" />
      ...
    </head>
   ```
5. External stylesheets are preferred to internal CSS when a single stylesheet needs to be linked to several html files. The use of a separate stylesheet then ensures that the code can be reused rather than repeated across multiple files.
6. A color hex code is a list of 6 hexidecimal digits which specifies the levels of red, green, and blue in a color. The first two characters of the code are a hexidecimal (base 16) number between 0 and 255 which specifies how much red should be included in the color. A level of 0 (00 in hexidecimal) indicates there is no red, and a level of FF (255) is the maximum level of red. Likewise, the third and fourth characters give the level of green in the color, and the fifth and sixth characters give the level of blue. For example, here are some colors and their corresponding hex codes:
  - red: `#FF0000`
  - green: `#00FF00`
  - blue: `#0000FF`
  - yellow: `#FFFF00`
  - violet: `#FF00FF`
  - cyan: `#00FFFF`
  - orange: `#FF8000`
7. The HSL color property is an alternative way of specifying a color. The letters in HSL stand for *hue*, *saturation*, and *lightness*. Hue specifies the shade of a color. It takes a value between 0 and 360. Saturation is the amount of gray in a color. It is specified by a percentage. A saturation of 0% entirely gray, whereas a saturation of 100% has no gray, and is thus fully *saturated* with its hue. Finally, lightness is the amount of white or black in a color. It is also expressed as a percentage. A lightness of 0% is black, and a lightness of 100% is white. The syntax for a color specified by hue, saturation, and lightness is
  ```    
   hsl(<hue>, <saturation>, <lightness>)
   ```
8. The three main categories of fonts are
   1. serif,
   2. sans-serif, and
   3. monospace.

   Serif fonts have small decorative additions to the ends of brush strokes called *serifs*. They were originally used in printed publications. Since computer screens have lower resolutions than can be achieved with printed text, serif fonts can be difficult to read when the font size is small. They are best used for headings and other large text.

   Sans-serif fonts are less elaborate than serif fonts. They are easier to read at small font sizes.

   Monospace fonts ensure that every letter is the same width. They are usually utilized when displaying code because they are considered to improve readability.
9. When specifying font sizes, the three main units used are
   1. pixels (`px`),
   2. percentages (`%`), and
   3. ems (`em`).
   Pixels give the height of each character in pixels with the px. For a given screen, the size of each letter will be fixed once specified in pixels. Since screen resolutions can vary though, a font size specified in pixels can look different on different devices.

    Percentages and ems are relative units. Percentages specify the font size of an element relative to the default font size of the browser, which is usually 16px. Ems are used to specify the font size of an element relative to the font size of its parent element.
