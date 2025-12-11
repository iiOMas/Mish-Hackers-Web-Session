# 🌐 Web Development 101: HTML & CSS Session

Welcome to your first step into Web Development! This session will cover the absolute basics of how websites are built.

## 🗺️ Roadmap

1.  **HTML Structure**: The skeleton of a page.
2.  **Text Formatting**: Headings, paragraphs, and styles.
3.  **Lists**: Organizing items.
4.  **Links & Images**: Connecting pages and adding visuals.
5.  **Basic CSS**: Making it look good.

---

## 🏗️ 01. HTML Structure

Every HTML page needs a standard "boilerplate" structure.

### 📝 Code Snippet

```html
<!DOCTYPE html>
<html>
  <head>
    <title>My First Page</title>
  </head>
  <body>
    <h1>Hello World!</h1>
  </body>
</html>
```

### 📂 File to Open

Go to `01-HTML-Structure/index.html` to see this in action.

### 🧠 Pop Quiz

<details>
<summary><strong>Question: Where does the content visible to the user go?</strong> (Click to reveal)</summary>
<blockquote>
Inside the <code>&lt;body&gt;</code> tag! Anything in <code>&lt;head&gt;</code> is just information for the browser (like the title).
</blockquote>
</details>

---

## ✍️ 02. Text Formatting

We use tags to tell the browser how to display text.

### Key Tags

- `<h1>` to `<h6>`: Headings (h1 is the biggest).
- `<p>`: Paragraphs.
- `<strong>`: **Bold** text.
- `<em>`: _Italic_ text.

### 📂 File to Open

Go to `02-Text-Formatting/index.html`.

### 🧠 Pop Quiz

<details>
<summary><strong>Question: How many levels of headings are there?</strong></summary>
<blockquote>
6 levels! From <code>&lt;h1&gt;</code> (most important) to <code>&lt;h6&gt;</code> (least important).
</blockquote>
</details>

---

## 📝 03. Lists

There are two main types of lists.

### 1. Unordered List (`<ul>`)

- Uses bullets.
- Good for shopping lists, features, etc.

### 2. Ordered List (`<ol>`)

- Uses numbers (1, 2, 3...).
- Good for recipes, instructions, steps.

### 📂 File to Open

Go to `03-Lists/index.html`.

### 🧠 Pop Quiz

<details>
<summary><strong>Question: Which tag is used for the list ITEMS inside the list?</strong></summary>
<blockquote>
The <code>&lt;li&gt;</code> tag (List Item). It goes inside both <code>&lt;ul&gt;</code> and <code>&lt;ol&gt;</code>.
</blockquote>
</details>

---

## 🔗 04. Links & Images

The web wouldn't be a "web" without links!

### Links (`<a>`)

```html
<a href="https://google.com">Go to Google</a>
```

- `href`: Valid "Hypertext Reference" (Where the link goes).

### Images (`<img>`)

```html
<img src="photo.jpg" alt="Description of photo" />
```

- `src`: Source (Where the file is).
- `alt`: Alternate text (If image fails to load or for screen readers).
- **Note**: `<img>` does NOT have a closing tag!

### 📂 File to Open

Go to `04-Links-and-Images/index.html`.

### 🧠 Pop Quiz

<details>
<summary><strong>Question: What attribute makes a link open in a new tab?</strong></summary>
<blockquote>
<code>target="_blank"</code>
</blockquote>
</details>

---

## 🎨 05. Basic CSS

HTML is structure. **CSS is Style.**

We can use a separate file called `styles.css` and link it to our HTML.

### How to Link

```html
<head>
  <link rel="stylesheet" href="styles.css" />
</head>
```

### CSS Syntax

```css
/* Selector */
h1 {
  color: blue; /* Property: Value */
  font-size: 50px;
}
```

### 📂 File to Open

Go to `05-Basic-CSS/index.html` and look at `styles.css`.

### 🧠 Pop Quiz

<details>
<summary><strong>Question: How do you select an element with `class="box"` in CSS?</strong></summary>
<blockquote>
By adding a dot! <code>.box { ... }</code>
</blockquote>
</details>

---

## 🚀 Final Challenge: Build a Profile Card!

**Goal**: Create a new file called `my-profile.html` and use everything we learned.

**Requirements:**

1.  [ ] An `<h1>` with your name.
2.  [ ] An `<img>` (your avatar or a placeholder).
3.  [ ] A short `<p>` bio about yourself.
4.  [ ] A `<ul>` list of your hobbies.
5.  [ ] A link `<a>` to your GitHub or LinkedIn.
6.  [ ] (Bonus) Add some CSS to make it look nice!

Good luck! 🎉
