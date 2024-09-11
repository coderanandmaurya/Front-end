### Tables, Semantic Elements, and Multimedia in HTML

#### Creating Tables in HTML

Tables are used in HTML to display tabular data. The structure of a table involves several key elements:

- **`<table>`**: Defines the table.
- **`<tr>`**: Defines a row in the table.
- **`<th>`**: Defines a header cell (typically bold and centered).
- **`<td>`**: Defines a standard data cell.
- **`<caption>`**: Provides a title or description for the table.

Example of a basic table:
```html
<table>
    <caption>Weekly Schedule</caption>
    <tr>
        <th>Day</th>
        <th>Activity</th>
    </tr>
    <tr>
        <td>Monday</td>
        <td>Yoga</td>
    </tr>
    <tr>
        <td>Tuesday</td>
        <td>Gym</td>
    </tr>
</table>
```

#### Table Attributes

1. **`colspan`**: Merges cells horizontally.
   ```html
   <td colspan="2">Merged Cell</td>
   ```

2. **`rowspan`**: Merges cells vertically.
   ```html
   <td rowspan="2">Merged Cell</td>
   ```

3. **Borders**: Table borders can be styled using CSS.
   ```html
   <style>
     table, th, td {
         border: 1px solid black;
         border-collapse: collapse;
     }
   </style>
   ```

#### Semantic Elements in HTML

Semantic elements define the structure of a webpage and make it more meaningful to search engines and assistive technologies.

- **`<header>`**: Represents the introductory content or navigation links.
- **`<footer>`**: Represents the footer content, such as copyright or contact information.
- **`<section>`**: Defines a standalone section of content.
- **`<article>`**: Represents independent content that could be distributed separately (e.g., a blog post).
- **`<aside>`**: Defines content related to the main content, such as sidebars.
- **`<nav>`**: Represents navigation links.

Example of a structured page with semantic elements:
```html
<header>
    <h1>Welcome to My Website</h1>
</header>

<nav>
    <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#contact">Contact</a></li>
    </ul>
</nav>

<section>
    <article>
        <h2>Latest News</h2>
        <p>Check out the latest news about technology.</p>
    </article>
</section>

<aside>
    <p>Sidebar content: advertisements, links, etc.</p>
</aside>

<footer>
    <p>&copy; 2024 My Website</p>
</footer>
```

#### Embedding Multimedia in HTML

Multimedia elements such as videos and audio files can be easily embedded in HTML.

- **`<audio>`**: Embeds audio files.
- **`<video>`**: Embeds video files.

##### `<audio>` Element

Example:
```html
<audio controls>
    <source src="audio-file.mp3" type="audio/mpeg">
    Your browser does not support the audio element.
</audio>
```

- **`controls`**: Adds play, pause, and volume controls for the user.

##### `<video>` Element

Example:
```html
<video controls width="400">
    <source src="video-file.mp4" type="video/mp4">
    Your browser does not support the video element.
</video>
```

- **`controls`**: Adds play, pause, and volume controls.
- **`width`**: Specifies the width of the video.

---

### Topics to Cover

#### Best Practices for Table Design

- Use tables **only** for tabular data, not for page layout.
- Ensure tables are **accessible** by using headers (`<th>`) to label columns and rows.
- Use **captions** to describe the content of the table.
- Make tables responsive by using CSS for styling rather than HTML attributes like `border` or `width`.

#### Importance of Semantic Elements for Accessibility and SEO

Semantic elements improve the **readability** of the HTML structure for both search engines (SEO) and screen readers (accessibility). They allow search engines to understand the content hierarchy and enable assistive technologies to better navigate the webpage.

---

### Practice

#### Create a Table to Display a Weekly Schedule

```html
<!DOCTYPE html>
<html>
<head>
    <title>Weekly Schedule</title>
    <style>
        table, th, td {
            border: 1px solid black;
            border-collapse: collapse;
            padding: 10px;
        }
    </style>
</head>
<body>
    <h1>Weekly Schedule</h1>
    <table>
        <caption>My Weekly Activities</caption>
        <tr>
            <th>Day</th>
            <th>Activity</th>
            <th>Time</th>
        </tr>
        <tr>
            <td>Monday</td>
            <td>Yoga</td>
            <td>8:00 AM</td>
        </tr>
        <tr>
            <td>Tuesday</td>
            <td>Gym</td>
            <td>6:00 PM</td>
        </tr>
        <tr>
            <td>Wednesday</td>
            <td>Swimming</td>
            <td>7:00 AM</td>
        </tr>
    </table>
</body>
</html>
```

#### Add a Video and an Audio File to Your Webpage

```html
<!DOCTYPE html>
<html>
<head>
    <title>Multimedia Example</title>
</head>
<body>
    <h1>Welcome to My Multimedia Page</h1>

    <h2>Watch this video:</h2>
    <video controls width="500">
        <source src="video.mp4" type="video/mp4">
        Your browser does not support the video tag.
    </video>

    <h2>Listen to this audio:</h2>
    <audio controls>
        <source src="audio.mp3" type="audio/mpeg">
        Your browser does not support the audio tag.
    </audio>
</body>
</html>
```

#### Use Semantic Elements to Structure a Webpage

```html
<!DOCTYPE html>
<html>
<head>
    <title>My Webpage with Semantic Elements</title>
</head>
<body>
    <header>
        <h1>Welcome to My Website</h1>
    </header>

    <nav>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <section>
        <h2>About Us</h2>
        <p>This is the about section of our website.</p>
    </section>

    <footer>
        <p>&copy; 2024 My Website</p>
    </footer>
</body>
</html>
```
