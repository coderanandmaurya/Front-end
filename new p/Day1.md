### What is HTML and How it Works

HTML (HyperText Markup Language) is the standard language used to create web pages. It provides the structure and content of a webpage by defining elements using tags. HTML works by using tags to mark up text, images, links, and other types of content that the web browser can then render.

When a web browser loads an HTML file, it interprets the tags and renders the content on the screen accordingly. HTML forms the basic building blocks of a webpage and can be extended with CSS (Cascading Style Sheets) for styling and JavaScript for interactive behavior.

### Structure of an HTML Document

An HTML document consists of several key elements that help structure its content:

- **`<!DOCTYPE html>`**: Declares the document type and version of HTML being used. It ensures the browser renders the page according to the correct standards.
- **`<html>`**: This is the root element that wraps all other HTML content.
- **`<head>`**: Contains metadata about the document such as its title, linked stylesheets, and scripts. It’s not visible to the user.
- **`<body>`**: Contains the visible content of the webpage, such as headings, paragraphs, images, etc.

### Basic Tags

1. **`<!DOCTYPE html>`**: Specifies the document is using HTML5.
2. **`<html>`**: The container for the entire HTML document.
3. **`<head>`**: Contains metadata like the document title (`<title>`) and links to external resources (e.g., CSS).
4. **`<body>`**: Holds the visible content that will be displayed on the webpage.

### Headings (`<h1>` to `<h6>`)

HTML defines six levels of headings, from `<h1>` (the most important) to `<h6>` (the least important). These headings are used to organize content hierarchically.

Example:
```html
<h1>Main Heading</h1>
<h2>Subheading</h2>
<h3>Sub-subheading</h3>
```

### Paragraphs (`<p>`)

Paragraphs are defined using the `<p>` tag and are used to group related sentences or content.

Example:
```html
<p>This is a paragraph of text in HTML.</p>
```

### Comments in HTML

Comments in HTML are added using `<!--` and `-->`. These are not visible to users but can help developers understand or organize code.

Example:
```html
<!-- This is a comment and will not be displayed in the browser -->
```

---

## Topics to Cover

### Creating Your First HTML Page

Here's how to create a basic HTML page:

```html
<!DOCTYPE html>
<html>
<head>
    <title>My First Web Page</title>
</head>
<body>
    <h1>Welcome to My Web Page</h1>
    <p>This is a simple HTML page.</p>
</body>
</html>
```

### Basic Text Formatting (Bold, Italic, Underline)

HTML allows basic text formatting using these tags:
- **Bold**: `<b>` or `<strong>`
- **Italic**: `<i>` or `<em>`
- **Underline**: `<u>`

Example:
```html
<p>This is <b>bold</b>, <i>italic</i>, and <u>underlined</u> text.</p>
```

### Inline vs Block Elements

- **Inline elements** do not start on a new line and only take up as much width as necessary (e.g., `<b>`, `<i>`, `<u>`).
- **Block elements** start on a new line and take up the full width available (e.g., `<p>`, `<div>`, `<h1>`).

---

## Practice

### Create a Simple "About Me" Page

Here's an example of an "About Me" page that uses basic HTML formatting:

```html
<!DOCTYPE html>
<html>
<head>
    <title>About Me</title>
</head>
<body>
    <h1>About Me</h1>
    <p>Hi, I'm Jane Doe. I love <b>coding</b>, <i>designing</i>, and exploring <u>new technologies</u>.</p>
</body>
</html>
```

### Experiment with Text Styling

You can play around with different text styles using `<b>`, `<i>`, and `<u>`:

```html
<p>My favorite hobby is <b>bold</b>, my passion is <i>italic</i>, and my goals are <u>underlined</u>.</p>
```
