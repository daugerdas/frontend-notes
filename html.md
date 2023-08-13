# Hyper Text Markup Language (HTML)

Introduction
Anatomy
Elements

## Introduction 
The Hyper Text Markup Language or HTML is the standard markup language for documents designed to be displayed in a web browser. The first version of HTML was written by Tim Berners-Lee in 1993. Since then, there have been many different versions of HTML.


## Anatomy
HTML consists of a series of elements. The element is the opening tag, followed by content, followed by the closing tag `<p>hello world</p>`.
| Opening tag | Content | Closing tag |
| --- | --- | --- |
| `<p>` | hello world | `</p>` |

HTML attributes provide additional information about HTML elements.The HTML class attribute is used to specify a class for an HTML element. Multiple HTML elements can share the same class. The class attribute is often used to point to a class name in a style sheet. It can also be used by a JavaScript to access and manipulate elements with the specific class name.
![Untitled-3](https://github.com/daugerdas/frontendintro.com/assets/14166408/ffebd742-65d9-49c9-bb9d-e135ecfe7ecf)

The text between <html> and </html> describes the web page, and the text between <body> and </body> is the visible page content. The markup text <title>This is a title</title> defines the browser page title shown on browser tabs and window titles. Between <head> and </head>, a <meta> element can be used to define webpage metadata. The Document Type Declaration <!DOCTYPE html> is for HTML5. If a declaration is not included, various browsers will revert to "quirks mode" for rendering.
![Untitled-4](https://github.com/daugerdas/frontendintro.com/assets/14166408/06f83f6b-53ee-4ef9-ad70-176e510b9bc5)


## Elements

- Meta elements - `title` defines the document's title that is shown in a browser's title bar or a page's tab. It only contains text; tags within the element are ignored, `meta` element represents metadata that cannot be represented by other HTML meta-related elements. Metadata is — in its very simplest definition — data that describes data. For example, an HTML document is data, `link` specifies relationships between the current document and an external resource., etc.
- Section elements - `article`, `header`, `footer`, `section`, `nav`, etc.
- Heading elements - `h1`-`h6`, `hgroup` element represents a multi-level heading for a section of a document, etc.
- Grouping elements - `main` element represents the dominant content of the `<body>` of a document., `p`, `ol`, `ul`, `dl` element represents a description list (specified using the description term `<dt>` element and `<dd>` description details elements), `figure` element represents self-contained content, potentially with an optional caption, which is specified using the (`<figcaption>`) element, `div`
- Table elements - `table`, `tr`, `td`, etc.
- Text elements - `em` element marks text that has stress emphasis, `br` element produces a line break in text (carriage-return), `mark` represents text which is marked or highlighted for reference or notation purposes, due to the marked passage's relevance or importance in the enclosing context, `abbr` represents an abbreviation or acronym; the optional title attribute can provide an expansion or description for the abbreviation, etc.

### Interactive elements

Interactive elements 
- Anchors
- Element forms - `form`, `input`, `select`, etc. 
- Embedded elements - `audio`, `iframe`, `img`, `svg`, `video`, `canvas`, etc.


### Majority of elements
| HTML Element and Tags | Description |
| --------------------- | ----------- |
| `<!DOCTYPE html>` | Defines that this document is an HTML5 document. All HTML documents must start with this declaration. This declaration is NOT case sensitive. |
| `<html>` | This element is the root element of an HTML page. Always include the lang attribute inside the <html> tag, to declare the language of the Web page. This is meant to assist search engines and browsers. |
| `<head>` | Contains meta information about the HTML page. This element is a container for the following elements: title, style, meta, link, script, and base. | 
| `<title>` | Specifies a title for HTML document and is required. |
| `<body>` | Defines the document's body, and is a container for all the visible contents, such as headings, paragraphs, images, hyperlinks, tables, lists, etc. |
| `<h1>` to `<h6>` |  Defines a large heading. h1 defines the most important heading. h6 defines the least important heading:  |
| `<p>` | Defines a paragraph. |
| `<a>` | Defines HTML link. The link's destination is specified in the href attribute. target attribute specifies where to open the linked document. Use the id attribute (id="value") to define bookmarks in a page. Use the href attribute (href="#value") to link to the bookmark. |
| `<img>` | Defines HTML images. The source file (src), alternative text (alt), width, and height are provided as attributes. The src attribute specifies the path to the image to be displayed. | 
| `<br>` | Inserts a single line break and defines a line break. It is an empty element without a closing tag. |
| `<hr>` | Defines a thematic break in an HTML page, and is most often displayed as a horizontal rule. This element is used to separate content (or define a change) in an HTML page. |
| `<pre>` | This element defines preformatted text. The text inside a pre element is displayed in a fixed-width font (usually Courier), and it preserves both spaces and line breaks. |
| `<b>` | Bold text |
| `<strong>` | Important text |
| `<i>` | Italic text |
| `<em>` | Emphasized text |
| `<mark>` | Marked text |
| `<small>` | Smaller text |
| `<del>` | Deleted text |
| `<ins>` | Inserted text |
| `<sub>` | Subscript text |
| `<sup>` | Superscript text |
| `<blockquote>` | Defines a section that is quoted from another source. |
| `<q>` | Defines a short quotation. |
| `<abbr>` | Defines an abbreviation or an acronym. |
| `<address>` | Defines the contact information for the author/owner of a document or an article. |
| `<cite>` | Defines the title of a creative work. | 
| `<bdo>` | Used to override the current text direction. |
| `<map>` | Defines an image map. An image map is an image with clickable areas. The areas are defined with one or more area tags. Use the HTML usemap attribute of the img element to point to an image map. |
| `<picture>` | This element allows you to display different pictures for different devices or screen sizes. The picture element contains one or more <source> elements, each referring to different images through the srcset attribute. Each source element has a media attribute that defines when the image is the most suitable. |
| `<link>` | Defines the relationship between a document and an external resource. Use the HTML link element to insert a favicon. This element is most often used to link to external style sheets. |
| `<table>` | Defines a table. |
| `<th>` | Defines a header cell in a table. | 
| `<tr>` | Defines a row in a table. |
| `<td>` | Defines a cell in a table. |
| `<caption>` | Defines a table caption. |
| `<colgroup>` | Specifies a group of one or more columns in a table for formatting. |
| `<col>` | Specifies column properties for each column within a colgroup element. |
| `<thead>` | Groups the header content in a table. |
| `<tbody>` | Groups the body content in a table. |
| `<tfoot>` | 	Groups the footer content in a table. |
| `<ul>` |	Defines an unordered list. The CSS list-style-type property is used to define the style of the list item marker. |
| `<ol>` |	Defines an ordered list. The type attribute of the ol tag, defines the type of the list item marker. |
| `<li>` |	Defines a list item. |
| `<dl>` |	Defines a description list. |
| `<dt>` |	Defines a term in a description list. |
| `<dd>` |	Describes the term in a description list. |
| `<div>` |  It is a block-level and is often used as a container for other HTML elements |
| `<span>` | It is an inline container used to mark up a part of a text, or a part of a document. |
| `<iframe>` | Specifies an inline frame. The src attribute defines the URL of the page to embed. |
| `<script>` |  This tag is used to define a client-side script. The script element either contains script statements, or it points to an external script file through the src attribute. | 
| `<noscript>` | Defines an alternate content to be displayed to users that have disabled scripts in their browser or have a browser that doesn't support scripts. |
| `<style>` | This element is used to define style information for a single document. |
| `<meta>` | This element is typically used to specify the character set, page description, keywords, author of the document, and viewport settings. |
| `<base>` | This element specifies the base URL and/or target for all relative URLs in a page. |
| `<header>` | Defines a header for a document or a section. |
| `<nav>` | Defines a set of navigation links. |
| `<section>` | Defines a section in a document. |
| `<article>` | Defines an independent, self-contained content. |
| `<aside>` | Defines content aside from the content (like a sidebar). |
| `<footer>` | Defines a footer for a document or a section. |
| `<details>` | Defines additional details that the user can open and close on demand. |
| `<summary>` | Defines a heading for the details element. |
| `<kbd>` | This element defines keyboard input. |
| `<samp>` | This element defines sample output from a computer program. |
| `<code>` | This element defines a piece of computer code. |
| `<var>` | This element defines a variable in programming or in a mathematical expression. |
| `<pre>` | This element defines preformatted text. |
| `<figcaption>` | Defines a caption for a figure element. |
| `<figure>` | Specifies self-contained content, like illustrations, diagrams, photos, code listings, etc. |
| `<main>` | Specifies the main content of a document. |
| `<time>` | Defines a date/time. |
| `<form>` | This element is used to create an HTML form for user input. The action attribute defines the action to be performed when the form is submitted. |
| `<input>` | Defines an input control. |
| `<textarea>` | Defines a multiline input control (text area). |
| `<label>` | Defines a label for an <input> element. |
| `<fieldset>` | Groups related elements in a form. |
| `<legend>` | Defines a caption for a fieldset element. |
| `<select>` | Defines a drop-down list. |
| `<optgroup>` | Defines a group of related options in a drop-down list. |
| `<option>` | Defines an option in a drop-down list. |
| `<button>` | Defines a clickable button. |
| `<datalist>` | Specifies a list of pre-defined options for input controls. |
| `<output>` | Defines the result of a calculation. |
| `<canvas>` |  Element is used to draw graphics via JavaScript. |
| `<svg>` | Element is a container for SVG graphics. |
| `<video>` | Element is used to show a video on a web page. |
| `<audio>` | 	Defines sound content. |
| `<source>` | Defines multiple media resources for media elements, such as video and audio. |
| `<object>` | Element defines an embedded object within an HTML document. |
| `<embed>` | Defines an embedded object within an HTML document. |
| `<!--...-->` | Defines a comment. |
| `<bdi>` | Isolates a part of text that might be formatted in a different direction from other text outside it. |
| `<data>` | Adds a machine-readable translation of a given content. |
| `<dfn>` | Specifies a term that is going to be defined within content. |
| `<dialog>` | Defines a dialog box or window. |
| `<meter>` | Defines a scalar measurement within a known range (a gauge). | 
| `<param>` | Defines a parameter for an object. |
| `<progress>` | Represents the progress of a task. |
| `<s>` | Defines text that is no longer correct. |
| `<template>` | Defines a container for content that should be hidden when the page loads. |
| `<track>` | Defines text tracks for media element (video and audio). |
| `<u>` | Defines some text that is unarticulated and styled differently from normal text. |
| `<wbr>` |  It specifies where in a text it would be ok to add a line-break. |
