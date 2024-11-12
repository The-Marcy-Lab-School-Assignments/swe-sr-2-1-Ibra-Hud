# Technical Writing Assignment

For guidance on setting up and submitting this assignment, refer to the Marcy lab School Docs How-To guide for [Working with Short Response and Coding Assignments](https://marcylabschool.gitbook.io/marcy-lab-school-docs/fullstack-curriculum/how-tos/working-with-assignments#how-to-work-on-assignments).

## Prompt 1

Do some research on semantic and non-semantic elements and share your findings. Your response should include:

- Examples of semantic and non-semantic tags
- The differences between semantic and non-semantic tags
- The benefits of using semantic tags (when possible)

### Response 1

Semantic tags provide context to the tags, i.e. footer would give the computer context so it'll be registered as the footer as well as helping other developers understand what a section is being used for. Utilizing semantic tags have numerous benefits one of which being SEO.

Non-Semantic tags are the opposite and are more ambiguous in relation to Semantic tags. The benefit of using semantic tags allow you more flexibility. Some examples of these tags:

```html
<!-- Semantic Tags -->
<article>
  <p>Article is one of those "Semantic" tags</p>
</article>

<!-- Non-Semantic Tags -->
<div>
  <p>Div is one of those "Non-Sematic" tags</p>
</div>
```

## Prompt 2

Do some research on accessibility. What are some ways to make your website more accessible? Explain why it is important for developers to create websites that meet accessibility standards.

### Response 2

Some ways to make your website accessible is to include alt tags (a way to add context to an image or video for screen readers) and to build screen reader and dyslexia accessibility features into your websites.

## Prompt 3

It is possible to add "inline" CSS styles to our html elements using the `style` attribute like so:

```html
<p style="color: red;">hello world</p>
```

While this is possible, it is a best practice to instead write styles in a separate CSS file. Provide at least one argument for why it _might_ be considered useful to write inline styles, and then provide a more compelling argument for writing styles in a separate CSS file.

### Response 3

A benefit of using inline CSS styles is best when doing quick checks and testing so a developer can see quick and automatic style changes without having to alter a CSS file.

Even though inline CSS isn't all bad it is better practice to use full CSS files. Using CSS files allows for better organization and more concise allowing for better maintainability as well as allowing for the file to be reused on other projects and pages.

## Prompt 4

Imagine you are teaching a brand new programmer a brief lesson about the `class` and `id` attributes in HTML as well as how to use them to style elements using CSS. Your lesson should have the following components:

- An explanation of the concept of "classes" and "ids" with an analogy.
- An example of the usage using an HTML code block and a CSS code block.
- An explanation of the syntax using the terms: **attribute**, **selector**

### Response 4

Html has many attributes that you can attribute to a html tag, two of which are the "class" and "id" tags. The class tag is an identifier attribute that allows you to call items with said class (the same class attribute can be used for different tags). i.e.

```html
<div class="example">
  <p>placeholder</p>
</div>
```

```css
.example {
  // This .example is a class selector
  color: blue;
}
```

As you see we accessed the class "example" in our css file by calling the class attribute. Our html code block (the first one) was used to define those values and create a paragraph with a section on our "website", while the CSS code block allows us to edit the visual representation of that code block. An example of ab id tag is this...

```html
<div id="example">
  <p>placeholder</p>
</div>
```

```css
#example {
  // This #example is an id selector
  color: blue;
}
```

With the id tag one thing we can do is link a button or rather link a link to a section of our application, which a class can also but do remember the id attribute is unique.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>Link Example</title>
  </head>
  <body>
    <!-- Link to the div with the id "example" -->
    <a href="#example">Go to Example Section</a>

    <!-- Some content to create space -->
    <p>Some content here...</p>
    <p>Some more content...</p>
    <p>Even more content...</p>

    <!-- Target div with the id "example" -->
    <div id="example">
      <p>placeholder</p>
    </div>
  </body>
</html>
```

## Prompt 5

The Document Object Model (DOM) API provides functions for manipulating HTML documents. It is possible to build an entire website using only JavaScript and the DOM API, however is that the best practice?

When building a website, how can I decide which content I should write using HTML/CSS and which content I should create using the JavaScript and the DOM API?

### Response 5

Though you can build a website using just JavaScript and the DOM API it is best practice to built projects with html/css as well. When building a website you want to use css for static content such as landing pages, blogs, about Me's, etc. these are our elements that for the most part wont change. Then you use css files for easy, readability, maintainability, and reusability. Allowing you to have similar pages (in regards to css) without having to recode it every time. Finally you want to use js and the dom api when you are building the interactive aspects of your websites, such as buttons, forms, etc. that has a lot of user input/interaction.
