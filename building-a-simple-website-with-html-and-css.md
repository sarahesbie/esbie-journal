# Building a Simple Website with HTML and CSS

## Setup:

1. **Download a code editor:** [VS Code](https://code.visualstudio.com/Download) / [Sublime Text](https://www.sublimetext.com/3) / [Atom](https://atom.io/)

Choosing a code editor comes down to personal preference - none are objectively 'better' than any others (although I'm sure a lot of developers will disagree with that sentiment). Do your research.

2. **Download a modern web browser**: [Chrome](#) / [Mozilla Firefox](#)

Whatever you do, don't use Internet Explorer.

3. **Download a website boilerplate:** https://github.com/sarahesbie/quickstart-site

No one needs to re-invent the wheel.

<hr/>

## Structuring your content with HTML

HTML stands for Hyper Text Markup Language. HTML (HyperText Markup Language) is the most basic building block of the Web. It defines the meaning and structure of web content. Other technologies besides HTML are generally used to describe a web page's appearance/presentation (CSS) or functionality/behavior (JavaScript).
"Hypertext" refers to links that connect web pages to one another, either within a single website or between websites. Links are a fundamental aspect of the Web. By uploading content to the Internet and linking it to pages created by other people, you become an active participant in the World Wide Web.

HTML uses "markup" to annotate text, images, and other content for display in a Web browser. HTML markup includes special "elements".

An HTML element is set off from other text in a document by "tags", which consist of the element name surrounded by "<" and ">".

### Step-by-step:

**1. Get set up...**

1. Open the website folder in VS Code
2. Open the website index.html file in your web browser
3. Open index.html file in VS Code

**2. Add some 'tags' in index.html**

Remember, tags are

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

- double-check the spelling of everything in your tag
- is the URL path to the image correct?
- do you have the right file extension for the image file?

4. Add more tags.

Go your hardest: https://www.w3schools.com/tags/default.asp

<hr/>

## Styling your content with CSS

Cascading Style Sheets (CSS) is a stylesheet language used to describe the presentation of a document written in HTML or XML (including XML dialects such as SVG, MathML or XHTML). CSS describes how elements should be rendered on screen, on paper, in speech, or on other media. CSS is one of the core languages of the open Web and is standardized across Web browsers according to the W3C specification.

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

**2. Add some styling rules in main.css**

1. Add some colour
2. Change the fonts

```
body {
    background-color:
}
```

3.

<hr/>

## Hosting your website on the Internet

- netlify
- domains
- how to find a web host, how to choose (what to look for - security, price, geography etc)

<hr/>
## Demos

- Here's a finished website on Github:
- And the same thing on Netlify:
