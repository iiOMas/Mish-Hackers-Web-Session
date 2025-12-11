# 🌐 Web Development 101

Welcome! Today we will learn how websites are built.

## 🧠 Part 1: The Concepts (Before we code)

Before writing code, we need to understand the **Legos** of the web.

### 1️⃣ What is a Tag?

A tag is a command to the browser. It starts with `<` and ends with `>`.

- **Example**: `<p>` tells the browser "Start a paragraph here".

### 2️⃣ What is an Element?

An element is the **whole thing**: The opening tag + The content inside + The closing tag.

```
  Element
  👇
<p> Hello World </p>
 👆      👆      👆
Tag    Content  Closing Tag
```

### 3️⃣ What is an Attribute?

Attributes are extra options we put _inside_ the opening tag.

- **Analogy**: If the tag is a "Car", the attribute is the "Color".
- **Code**: `<p class="big-text">` (Here, `class` is the attribute).

---

## 🏗️ Part 2: The Structure

Now let's look at the file `01-HTML-Structure/index.html`.

Every file needs a skeleton:

1.  **`<!DOCTYPE html>`**: Says "I am a modern website".
2.  **`<html>`**: The box holding everything.
3.  **`<head>`**: The **Brain** (Settings, Title). Users don't see this.
4.  **`<body>`**: The **Body** (Text, Images). Users SEE this.

**🗣️ Ask**: Where would I put my photo? In the head or the body?

---

## ✍️ Part 3: Text Formatting

Open `02-Text-Formatting/index.html`.

We use tags to change how text looks.

- `<h1>` is a **Headline** (Big and bold).
- `<p>` is a **Paragraph** (Normal text).
- `<strong>` makes text **Bold**.
- `<em>` makes text _Italic_.

**🗣️ Ask**: If `h1` is the biggest headline, what do you think is the smallest?

---

## 📝 Part 4: Lists

Open `03-Lists/index.html`.

- **Ordered List (`<ol>`)**: Numbered (1, 2, 3). Used for recipes/steps.
- **Unordered List (`<ul>`)**: Bullet points. Used for features/items.
- **List Item (`<li>`)**: The actual item inside the list.

---

## 🔗 Part 5: Links & Images

Open `04-Links-and-Images/index.html`.

### Links (`<a>`)

The "Anchor" tag connects pages.

```html
<a href="google.com">Click me</a>
```

- **Note**: `href` is an **Attribute**!

### Images (`<img>`)

```html
<img src="cat.jpg" alt="A cute cat" />
```

- **Note**: Images don't have a closing tag! They are "Self-Closing".

**🗣️ Ask**: Why doesn't an image need a closing tag like `</img>`? (Hint: Does it have text inside it?)

---

## 🎨 Part 6: Basic CSS

Open `05-Basic-CSS/index.html`.

HTML is the **Skeleton**. CSS is the **Skin/Clothes**.

We select elements and give them styles:

```css
/* Selector { Property: Value; } */
p {
  color: red;
}
```

- **Color**: Text color.
- **Background-color**: Background color.
- **Font-size**: How big the text is.

---

## 🚀 Challenge: Build Your Profile

Create a new file `profile.html`:

1.  Add an `<h1>` with your name.
2.  Add a `<p>` with your job/title.
3.  Add a `<ul>` of 3 things you like.
4.  Add an `<a>` link to your favorite website.
