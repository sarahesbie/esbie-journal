# Building a Simple Website with HTML and CSS

## Setup:

1. **Download and open a code editor:** [VS Code](https://code.visualstudio.com/Download) / [Sublime Text](https://www.sublimetext.com/3) / [Atom](https://atom.io/)

Choosing a code editor comes down to personal preference - none are objectively 'better' than any others (although I'm sure a lot of developers will disagree with that sentiment). Do your research.

2. **Download a modern web browser**: [Chrome](https://www.google.com/chrome/) / [Mozilla Firefox](https://www.mozilla.org/en-US/firefox/new/)

Just don't use Internet Explorer.

3. **Download a website boilerplate:** https://github.com/sarahesbie/quickstart-site

No one needs to re-invent the wheel.

<hr/>

## Coding in HTML

HTML stands for Hyper Text Markup Language. "Hypertext" refers to links that connect web pages to one another, either within a single website or between websites. "Markup" is used to annotate text, images, and other content for display in a Web browser. HTML markup includes special "elements".

An HTML element is set off from other text in a document by "tags", which consist of the element name surrounded by "<" and ">".

An HTML element can be made up of several components, including:

- An opening tag
- One or more tag attributes and corresponding values
- Tag content
- A closing tag

_Tip: HTML tags are written in lowercase_

Here are some examples:

`<p>This is some paragraph text. Paragraphs are block-level elements. Paragraphs can span multiple lines, and do not contain any line breaks.<p>`

`<a href="https://southstart.co/">Visit the _southstart website!</a>`

_Tip: some HTML tags are self closing_

`<img src="./images/my-example-image.jpg" alt="an example of an image"/>`

_Tip: tags can be nested inside eachother_

```
<nav class="main-nav">
    <a href="./page-1.html">Page One</a>
    <a href="./page-2.html">Page Two</a>
</nav>
```

Here's a full HTML tag reference: https://www.w3schools.com/tags/

### HTML step-by-step:

**1. Get set up...**

1. Download a boilerplate or create a new folder on your computer
2. Open the website folder in VS Code
3. In VS Code, either open index.html file from your boilerplate, or create a new file called index.html
4. Open the website index.html file in your web browser

_Tip: index.html is the default file name for a website's home page - the home page serves as an 'index' to the main pages on the site, each of which can link to any number of other pages._

**2. Add some HTML elements in index.html**

1. Add a first-level heading using `<h1>` tags:

   `<h1> This is the most important heading on my page </h1>`

2. Add a paragraph using `<p>` tags

   `<p> This is some paragraph text. Paragraphs are block-level elements. Paragraphs can span multiple lines, and do not contain any line breaks. <p>`

3. Add an image using the `<img/>` tag

The `<img>` tag is empty, it contains attributes only, and does not have a closing tag.

The src attribute specifies the URL (web address) of the image. If not specified, the browser expects to find the image in the same folder as the web page.

However, it is common to store images in a sub-folder. You must then include the folder name in the src attribute:

The alt attribute provides an alternate text for an image, if the user for some reason cannot view it (because of slow connection, an error in the src attribute, or if the user uses a screen reader).

`<img src="./images/my-example-image.jpg" alt="an example of an image"/>`

_Troubleshooting: why doesn't my image show up?_

- double-check the spelling of everything in your element
- double-check the file name
- is the URL path to the image correct?
- do you have the right file extension for the image file?

4. Add a link using the `<a>` tag

The `<a>` tag defines a hyperlink, which is used to link from one page to another (either within the same website, or anywhere else on the web). The most important attribute of the `<a>` element is the _href_ attribute, which indicates the link's destination.

`<a href="https://southstart.co/">Visit the _southstart website!</a>`

5. Add more tags - go your hardest!

Full tag reference: https://www.w3schools.com/tags/default.asp

Suggestions:

- a bulleted list
- a numbered list
- different level headings
- a horizontal line

<hr/>

## Styling your content with CSS

Cascading Style Sheets (CSS) is a stylesheet language used to describe the presentation of a document written in HTML.

A CSS rule is made up of several components:

- A selector - outside of the curly brackets
- A declaration - inside of the curly brackets
- A property - to the left of the colon
- One or more values - to the right of the colon

Here are some examples:

`p {color: purple;}`

`body { background-color:#999; }`

`img { width: 60%; }`

`a { text-decoration: underline }`

Here's the full CSS reference: https://www.w3schools.com/cssref/

### CSS step-by-step:

**1. Get set up...**

1. Open the website folder in VS Code
2. Open the website index.html file in your web browser
3. Open the main.css file in VS Code
4. Open the index.html file in VS Code and ensure the main stylesheet is linked. In order for your styling rules from main.css to apply, your page must include a reference to the external style sheet file (main.css) inside the <link> element, inside the head section.

```
<!DOCTYPE html>
<html>
    <head>
        <link rel="stylesheet" type="text/css" href="main.css">
    </head>
    <body>
        <p>This is a paragraph<p/>
    </body>
</html>
```

**2. Add styling rules in your css file**

1. Add colour

In CSS, colors are specified using predefined color names, or RGB, HEX, HSL, RGBA, HSLA values. Each of the below variations will have the same result in the browser:

`background-color: tomato;`

`background-color: rgb(255, 99, 71);`

`background-color:#ff6347;`

`background-color: hsl(9, 100%, 64%);`

More about CSS colour models:
https://www.w3schools.com/css/css_colors.asp

Colour can be applied using the following properties:

- `background-color` - sets a background colour for HTML elements
- `color` - sets the colour for text elements
- `border-color` - sets the colour of borders

_Tip: in CSS, color is always written in American English_

2. Change the font styles

The CSS font properties define the font family, boldness, size, and the style of a text.

Try the following properties:

- font-family: specifies the font family for text
- font-size: specifies the font size of text
- font-style: specifies the font style for text

```
p {
    font-family: 'Courier New', monospace;
    font-size:18px;
    font-style: italic;
}
```

There are a number of 'web safe fonts' that will display on any browser. For more font choices, check out [Google Fonts](https://www.w3schools.com/howto/howto_google_fonts.asp)

Web safe font examples:

`font-family: "Times New Roman", Times, serif;`

`font-family: Arial, Helvetica, sans-serif;`

`font-family: "Lucida Sans Unicode", "Lucida Grande", sans-serif;`

`font-family: "Courier New", Courier, monospace`

Full font reference here: https://www.w3schools.com/css/css_font.asp

3. CSS has so many possibilities. What else can you style?

- border
- width
- margin
- padding
- text transform (uppercase and lowercase)

Here's the full CSS reference: https://www.w3schools.com/cssref/

<hr/>
<!-- 
## Hosting your website on the Internet
<!- netlify
- domains
- how to find a web host, how to choose (what to look for - security, price, geography etc) 
-->

## Demos

- Here's a finished website on Github: https://github.com/sarahesbie/example-html-css-website
- And the same thing on Netlify: https://dreamy-fermat-d336ab.netlify.com/
