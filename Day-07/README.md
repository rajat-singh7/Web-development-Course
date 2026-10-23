 ## 1. What Are Semantic Tags?
**Semantic HTML tags are HTML elements that clearly describe the meaning and purpose of their content.**

The word *semantic* means related to meaning.

For example:

```html
<header>
    <h1>My Website</h1>
</header>

<nav>
    <a href="/">Home</a>
    <a href="/about">About</a>
</nav>

<main>
    <article>
        <h2>Learning HTML</h2>
        <p>HTML provides the structure of a webpage.</p>
    </article>
</main>

<footer>
    <p>Copyright 2026 My Website</p>
</footer>
```

From the tags themselves, we can understand which section contains the page header, navigation, main content, article, and footer.

Semantic tags were introduced as part of the evolution of HTML, with many important structural elements added in HTML5.

### Why is semantic HTML important?

Semantic HTML helps:

- Developers understand the structure of a webpage.
- Browsers identify the purpose of different elements.
- Screen readers communicate page structure to users.
- Search engines better understand the content and its organization.
- Teams maintain and update code more easily.

**Remember:** Semantic HTML describes the meaning of content, not its visual appearance.
## 2. Why Do We Use Semantic Tags?

Consider two ways to create a website header.

### Using non-semantic elements

```html
<div class="header">
    <h1>My Website</h1>
</div>

<div class="navigation">
    <a href="/">Home</a>
    <a href="/about">About</a>
</div>
```

### Using semantic elements

```html
<header>
    <h1>My Website</h1>
</header>

<nav>
    <a href="/">Home</a>
    <a href="/about">About</a>
</nav>
```

Both examples can look identical after CSS is applied.

However, the second example communicates the purpose of each section directly through HTML.

### Main advantages

1. **Readability:** The structure is easier to understand.
2. **Accessibility:** Assistive technologies can identify meaningful page landmarks.
3. **SEO:** Clear content structure can help search engines interpret a page.
4. **Maintainability:** Developers can understand and modify code more easily.
5. **Consistency:** Semantic elements provide a common structure for web documents.

---

## 3. Semantic vs Non-Semantic Tags

| Semantic tags | Non-semantic tags |
|---|---|
| `<header>` | `<div>` |
| `<nav>` | `<div>` |
| `<main>` | `<div>` |
| `<article>` | `<div>` |
| `<section>` | `<div>` |
| `<footer>` | `<div>` |
| `<aside>` | `<div>` |

### Semantic example

```html
<article>
    <h2>Introduction to CSS</h2>
    <p>CSS is used to style web pages.</p>
</article>
```

The `<article>` element indicates that the content is a self-contained piece of content.

### Non-semantic example

```html
<div class="article">
    <h2>Introduction to CSS</h2>
    <p>CSS is used to style web pages.</p>
</div>
```

Here, the browser does not receive the same semantic meaning from `<div>` itself. The class name `article` is primarily a label for CSS and scripts.

**Important:** Non-semantic elements are not bad. `<div>` and `<span>` remain useful when no more appropriate semantic element exists.

---

## 4. Important Semantic Tags

### 4.1 `<header>`

The `<header>` element represents introductory content for a page or a section.

It commonly contains:

- A website logo.
- A heading.
- Introductory text.
- Search controls.
- Other introductory elements.

Example:

```html
<header>
    <h1>CodeWithMe</h1>
    <p>Learn web development step by step.</p>
</header>

4.2 <nav>

The <nav> element represents a major group of navigation links.

Example:

```html
<nav>
    <a href="index.html">Home</a>
    <a href="about.html">About</a>
    <a href="contact.html">Contact</a>
</nav>
```

Use `<nav>` for important navigation areas, such as a primary menu or table of contents.

Not every individual link needs to be inside a `<nav>` element.

### 4.3 `<main>`

The `<main>` element represents the dominant content of the document's body.

Example:

```html
<main>
    <h1>Welcome to My Website</h1>
    <p>This is the main content of the page.</p>
</main>
```

Best practices:

- Usually use one visible `<main>` element per page.
- Do not place repeated site-wide content, such as the common navigation menu, inside `<main>`.
- The main content should be the central focus of the page.

### 4.4 `<section>`

The `<section>` element represents a thematic grouping of content.

Example:
<section>
    <h2>Our Services</h2>
    <p>We provide web development services.</p>
</section>
Use `<section>` when the content forms a meaningful topic or part of the document.
A section will often have a heading.

Do not use `<section>` merely to create a styling container. Use `<div>` when the grouping has no particular semantic meaning.

### 4.5 `<article>`

The `<article>` element represents self-contained content that can make sense independently.

Examples include:

- Blog posts.
- News articles.
- Forum posts.
- Product reviews.
- Independent user-submitted content.

Example:

```html
<article>
    <h2>What Is HTML?</h2>
    <p>HTML defines the structure of web content.</p>
</article>
```

An article may have its own `<header>` and `<footer>`.

### 4.6 `<aside>`

The `<aside>` element represents content that is related to the surrounding content but is not part of its main flow.

Examples:

- Related articles.
- A sidebar.
- Additional notes.
- Supplementary resources.

Example:

```html
<aside>
    <h2>Related Topics</h2>
    <ul>
        <li>HTML Basics</li>
        <li>CSS Basics</li>
    </ul>
</aside>
```

The exact placement of `<aside>` depends on whether the supplementary content relates to the entire page or a particular section.

### 4.7 `<footer>`

The `<footer>` element represents footer information for a page or section.

It can contain:

- Copyright information.
- Author details.
- Related links.
- Contact information.
- Additional navigation.

Example:

```html
<footer>
    <p>&copy; 2026 CodeWithMe</p>
    <a href="contact.html">Contact Us</a>
</footer>
```

A webpage can have multiple footers, for example, one for the overall website and another for a particular article.

### 4.8 `<figure>` and `<figcaption>`

`<figure>` represents self-contained content, such as an illustration, diagram, code example, or photograph.

`<figcaption>` provides a caption for that content.

Example:

```html
<figure>
    <img src="html-structure.png" alt="Diagram showing HTML document structure">
    <figcaption>Basic structure of an HTML document.</figcaption>
</figure>
```

The caption is optional. It can appear before or after the main content inside `<figure>`.

### 4.9 `<details>` and `<summary>`

`<details>` creates a disclosure widget that users can expand or collapse.

`<summary>` provides the visible label for that widget.

Example:

```html
<details>
    <summary>What is semantic HTML?</summary>
    <p>Semantic HTML uses elements that describe their content's meaning.</p>
</details>
```

The browser provides the basic expand-and-collapse behavior without requiring JavaScript.

### 4.10 `<time>`

The `<time>` element represents a date, time, or duration in a machine-readable format when appropriate.

Example:

```html
<p>
    Published on
    <time datetime="2026-10-23">October 23, 2026</time>.
</p>
```

The `datetime` attribute provides a machine-readable value.

### 4.11 `<address>`

The `<address>` element represents contact information for the relevant person, organization, or article.

Example:

```html
<address>
    Contact: <a href="mailto:hello@example.com">hello@example.com</a>
</address>
```

It is not intended for every ordinary postal address appearing in an article.

### 4.12 `<blockquote>` and `<q>`

`<blockquote>` represents an extended quotation.

`<q>` represents a short, inline quotation.

Example:

```html
<blockquote>
    <p>Learning is a continuous process.</p>
</blockquote>

<p>The teacher said, <q>Practice makes progress.</q></p>
```

Browsers commonly display quotation marks or indentation, but the main purpose of these elements is to identify quoted content.

### 4.13 `<mark>`

`<mark>` represents text highlighted because it is relevant in the current context.

Example:

```html
<p>Remember the term <mark>semantic HTML</mark> for revision.</p>
```

It is useful for highlighting relevant passages, search matches, or important text in context.

### 4.14 `<strong>` and `<em>`

`<strong>` indicates strong importance, seriousness, or urgency.

`<em>` indicates stress emphasis that can affect the meaning of a sentence.

Example:

```html
<p><strong>Important:</strong> Save your work regularly.</p>

<p>You <em>must</em> submit the assignment today.</p>
```

They commonly appear bold and italic, respectively, in browsers' default styles, but their meanings are not limited to those visual appearances.

### 4.15 `<abbr>`

`<abbr>` represents an abbreviation or acronym.

Example:

```html
<p>
    <abbr title="HyperText Markup Language">HTML</abbr>
    defines the structure of web pages.
</p>
```

The `title` attribute can provide the expanded form. It is optional, and support for displaying the tooltip varies by device and browser.

### 4.16 `<cite>`

`<cite>` represents the title of a creative work, such as a book, film, report, or website.

Example:

```html
<p>
    One useful reference is
    <cite>Learning Web Design</cite>.
</p>
```

It is not intended merely to identify the name of a person who said a quotation.

### 4.17 `<data>`

`<data>` connects human-readable content with a machine-readable value.

Example:

```html
<p>
    Product:
    <data value="P101">Wireless Mouse</data>
</p>
```

The visible product name is intended for people, while the `value` attribute provides a corresponding machine-readable value.

### 4.18 `<output>`

`<output>` represents the result of a calculation or user action.

Example:

```html
<form oninput="result.value = Number(a.value) + Number(b.value)">
    <input type="number" name="a" value="2">
    +
    <input type="number" name="b" value="3">
    =
    <output name="result">5</output>
</form>
```

Here, the `<output>` element displays the result. This example uses inline JavaScript through the form's `oninput` attribute.

---

## 5. Complete HTML Page Example

The following example combines several important semantic elements into a single webpage.

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="A beginner-friendly guide to semantic HTML.">

    <title>Semantic HTML Guide</title>
</head>

<body>

    <header>
        <h1>My Learning Website</h1>
        <p>Learn HTML, CSS, and JavaScript.</p>
    </header>

    <nav aria-label="Main navigation">
        <a href="#home">Home</a>
        <a href="#articles">Articles</a>
        <a href="#contact">Contact</a>
    </nav>

    <main id="home">

        <section>
            <h2>Welcome</h2>
            <p>Explore the fundamentals of web development.</p>
        </section>

        <section id="articles">
            <h2>Latest Articles</h2>

            <article>
                <header>
                    <h3>Introduction to HTML</h3>
                    <p>
                        Published on
                        <time datetime="2026-10-23">October 23, 2026</time>
                    </p>
                </header>

                <p>
                    HTML provides the structure and meaning
                    of content on a webpage.
                </p>

                <figure>
                    <img src="html-example.png"
                         alt="Example of an HTML document structure">
                    <figcaption>Example of semantic HTML structure.</figcaption>
                </figure>

                <footer>
                    <p>Category: Web Development</p>
                </footer>
            </article>

        </section>

        <aside>
            <h2>Related Topics</h2>
            <ul>
                <li>CSS Selectors</li>
                <li>HTML Forms</li>
                <li>JavaScript Basics</li>
            </ul>
        </aside>

    </main>

    <footer id="contact">
        <p>&copy; 2026 My Learning Website</p>
        <address>
            <a href="mailto:hello@example.com">Contact Us</a>
        </address>
    </footer>

</body>
</html>
```

### Understanding the structure

- `<header>` introduces the website.
- `<nav>` groups the primary navigation links.
- `<main>` identifies the primary page content.
- `<section>` groups content by topic.
- `<article>` contains a self-contained article.
- `<time>` identifies a publication date.
- `<figure>` and `<figcaption>` associate an image with a caption.
- `<aside>` contains supplementary resources.
- `<footer>` contains footer information.