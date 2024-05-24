# Repetition of HTML and CSS

<details>
<summary>Table of contents</summary>

- [HTML Repetition](#html-repetition)
  - [Semantics](#semantics)
    - [Importance of Semantics in HTML](#importance-of-semantics-in-html)
    - [Examples of Semantic HTML Elements](#examples-of-semantic-html-elements)
- [CSS Repetition](#css-repetition)
  - [What is CSS?](#what-is-css)
  - [CSS syntax](#css-repetition)
  - [Three different ways to style your content](#three-different-ways-to-style-your-content)
    - [Element styling](#element-styling)
    - [Class styling](#class-styling)
    - [Id styling](#id-styling)
- [Box-model](#box-model)
  - [Components of the Box Model](#components-of-the-box-model)
  - [Box-sizing](#box-sizing)

</details>

## HTML Repetition

### Semantics

As a beginner, understanding semantics in HTML is crucial for creating well-structured and meaningful web documents. In HTML, semantics refer to the meaning or purpose of the elements used to structure a web page's content. Semantic HTML elements provide a clear and descriptive outline of the content's structure, making it easier for both humans and machines (such as search engines and screen readers) to understand the purpose of each part of the document.

#### Importance of Semantics in HTML

- Clarity and Readability: Semantic HTML elements help developers and other collaborators understand the structure and purpose of a webpage's content more easily. This clarity improves readability and facilitates collaboration during development and maintenance.

- Accessibility: Semantic HTML enhances accessibility by providing meaningful structure to web content. Screen readers and other assistive technologies rely on semantic elements to interpret and present content to users with disabilities.

- Search Engine Optimization (SEO): Search engines use semantic HTML to understand the content and context of web pages better. Proper use of semantic elements can improve a webpage's search engine ranking and visibility.

#### Examples of Semantic HTML Elements

- `<header>`: Represents introductory content or a set of navigational links for its nearest ancestor sectioning content or sectioning root.

- `<nav>`: Represents a section of the document intended for navigation links.

- `<section>`: Represents a thematic grouping of content, typically with a heading. It is used to divide the document into sections with related content.

- `<article>`: Represents a self-contained piece of content that could be independently distributed or reused, such as a blog post, news article, or forum post.

- `<footer>`: Represents a footer for its nearest sectioning content or sectioning root element.

- `<p>`: Represents a paragraph of text. It is a block-level element used to group sentences and provide structure to text content.

- ` <h1>, <h2>, <h3>` and so on: Heading elements represent headings of varying levels of importance, with `<h1>` being the most important and `<h6>` being the least important.

[Back to top](#repetition-of-html-and-css)

## CSS Repetition

### What is CSS?

CSS stands for cascading style sheet. It says nothing really but it means tha styling always cascades down through the css stylesheet. CSS goes from top to bottom so the structure in your css stylesheets matters.

### CSS syntax

  <figure>
    <img src="./images/img_selector.gif">
  </figure>

- **Selector:** Targets the element that we want to style. Be specific here , the more the merrier.

- **Declaration:** It's a combination of a property and value.

- **Property:** The specific styling that we want to apply to the element specified by the selector. Could be `background-color`, `margin`, `padding` and so on.

- **Value:** It's the value that we give to the property and is the thing that is visible on the webpage. For instance, the color red for the background color: `background-color: red`

The syntax for css looks like this:

```css
selector {
  css-rule: value;
}
```

Let's look at the selector syntax:

```css
/* element selector */
h1 {
  color: white;
}

/* class selector, using period ( . ) */
.some-class {
  color: red;
}

/* id selector, using ( # ) */
#some-id {
  color: green;
}
```

[Back to top](#repetition-of-html-and-css)

### Three different ways to style your content.

- Styling with HTML Elements: Directly applies styles to all elements of the specified type.

- Styling with Classes: Groups multiple elements together and applies styles collectively.

- Styling with IDs: Applies specific styles to individual elements based on their unique identifiers.

Each method has its own use cases and advantages. Classes are often used for reusable styles applied to multiple elements, while IDs are used for unique styling or JavaScript targeting. It's important to choose the appropriate method based on your styling requirements and the structure of your HTML document.

[Back to top](#repetition-of-html-and-css)

#### Element styling

It is styling that targets a specific html element. Could be the `<h1>` tag for instance. But remember, if you style this way, **ALL** the `<h1>` tags will get the same styling. It's not very specific in other words.

```css
h1 {
  color: blue;
  /* All h1 elements will be blue in this case */
}
```

[Back to top](#repetition-of-html-and-css)

#### Class styling

Class styling is used when we want to be much more specific on which element to style. There might be several of the same kind, but we are only interested in styling on of those. Then we use a css class.

```css
.some-class {
  background-color: blue;
  /* This styling will only apply to an element that has the specific class "some-class". */
}
```

A good thing to know about classes is that you can resuse them as many times as you want.

[Back to top](#repetition-of-html-and-css)

#### Id styling

Works the same was as a class, you just use `#` instead. The convention here is that the id is unique, it means you shouldn't reuse it in the same document.

```css
#some-id {
  background-color: yellow;
  /* This styling will only apply on the element that has the id of "some-id"; */
}
```

[Back to top](#repetition-of-html-and-css)

### Box-model

<figure><img src="./images/box_model.png"></figure>

The CSS box model is a fundamental concept that describes how elements are rendered on a web page, specifically how their content, padding, border, and margin interact to determine their overall size and appearance. Understanding the box model is crucial for controlling the layout and spacing of elements on a webpage.

#### Components of the Box Model

- Content: This is the actual content of the element, such as text, images, or other media. It is defined by the width and height properties.

- Padding: Padding is the space between the content and the element's border. It helps create space around the content and improves readability. Padding is specified using the padding property.

- Border: The border surrounds the padding and content of the element. It is defined by the border property, which includes properties for specifying the border width, style, and color.

- Margin: Margin is the space outside the border of the element. It creates space between elements and helps control the layout of the page. Margin is specified using the margin property.

[Back to top](#repetition-of-html-and-css)

#### Box-sizing

By default, the width and height properties in CSS apply to the content area only. However, you can change this behavior using the box-sizing property. Setting box-sizing: border-box; includes padding and border in the element's total width and height.

[Back to top](#repetition-of-html-and-css)
