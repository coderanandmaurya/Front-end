### HTML Links, Images, and Lists

#### Adding Links with the `<a>` Tag
HTML links are created using the `<a>` tag, which stands for "anchor." Links can either be **internal** (linking to other pages within the same website) or **external** (linking to other websites).

- **Internal Link**: Links to another section or page of the same website.
  ```html
  <a href="about.html">About Us</a>
  ```

- **External Link**: Links to an external website.
  ```html
  <a href="https://www.example.com">Visit Example</a>
  ```

- **Opening in a new tab**: Use the `target="_blank"` attribute to open links in a new tab.
  ```html
  <a href="https://www.example.com" target="_blank">Visit Example</a>
  ```

#### Adding Images with the `<img>` Tag

Images are added to a webpage using the `<img>` tag. It is a **self-closing tag**, meaning it doesn’t need a closing tag. Key attributes include:
- **`src`** (source): Specifies the image location (either relative or absolute URL).
- **`alt`** (alternative text): Describes the image for accessibility and when the image can't be displayed.

Example:
```html
<img src="images/picture.jpg" alt="A beautiful landscape" />
```

##### Image Paths:
- **Relative Path**: Refers to a file within the same project or website.
  ```html
  <img src="images/photo.jpg" alt="A photo" />
  ```
- **Absolute Path**: A full URL to an image.
  ```html
  <img src="https://example.com/photo.jpg" alt="A photo from a website" />
  ```

#### Types of Lists

1. **Ordered List** (`<ol>`): Displays a numbered list.
   ```html
   <ol>
     <li>Item One</li>
     <li>Item Two</li>
     <li>Item Three</li>
   </ol>
   ```

2. **Unordered List** (`<ul>`): Displays a bulleted list.
   ```html
   <ul>
     <li>Item One</li>
     <li>Item Two</li>
     <li>Item Three</li>
   </ul>
   ```

#### Nesting Lists

Lists can be nested by placing one list inside an `<li>` element of another list.

Example:
```html
<ul>
  <li>Item One</li>
  <li>Item Two
    <ul>
      <li>Sub-item A</li>
      <li>Sub-item B</li>
    </ul>
  </li>
  <li>Item Three</li>
</ul>
```

---

## Topics to Cover

### Attributes (href, src, alt, target, etc.)

Attributes provide additional information about HTML elements. Some common attributes include:
- **`href`**: Specifies the URL for links (`<a>`).
- **`src`**: Specifies the image file location (`<img>`).
- **`alt`**: Describes the content of an image for accessibility (`<img>`).
- **`target`**: Specifies where to open the linked document (`<a>`).
- **`title`**: Adds a tooltip when hovering over an element.

### Image Paths (Relative and Absolute)
- **Relative Path**: Refers to the file location within the website's directory structure.
- **Absolute Path**: Refers to a complete URL of a resource (typically external).

---

## Practice

### Create a Webpage with Navigation Links to Different Sections

Example:
```html
<!DOCTYPE html>
<html>
<head>
    <title>My Webpage</title>
</head>
<body>
    <nav>
        <ul>
            <li><a href="#about">About Me</a></li>
            <li><a href="#hobbies">My Hobbies</a></li>
            <li><a href="contact.html">Contact</a></li>
        </ul>
    </nav>

    <h2 id="about">About Me</h2>
    <p>Hello! I'm a web developer passionate about technology.</p>

    <h2 id="hobbies">My Hobbies</h2>
    <p>I enjoy reading, hiking, and coding.</p>
</body>
</html>
```

### Add Images to Your Webpage with Proper Alt Text for Accessibility

Example:
```html
<!DOCTYPE html>
<html>
<head>
    <title>My Photo Gallery</title>
</head>
<body>
    <h1>My Favorite Photos</h1>

    <img src="images/mountain.jpg" alt="A beautiful mountain view" />
    <img src="images/beach.jpg" alt="A sunny beach" />
</body>
</html>
```

### Create an Ordered and Unordered List

Example:
```html
<!DOCTYPE html>
<html>
<head>
    <title>My Lists</title>
</head>
<body>
    <h2>Ordered List - Favorite Books</h2>
    <ol>
        <li>1984 by George Orwell</li>
        <li>The Great Gatsby by F. Scott Fitzgerald</li>
        <li>To Kill a Mockingbird by Harper Lee</li>
    </ol>

    <h2>Unordered List - Hobbies</h2>
    <ul>
        <li>Reading</li>
        <li>Hiking</li>
        <li>Traveling</li>
    </ul>
</body>
</html>
```
