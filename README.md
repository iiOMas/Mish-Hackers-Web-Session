# HTML Basics — Session Notes

Welcome! concepts are explained in Arabic/English below.

👉 **Section 1 — What is HTML?**

<details>
<summary><strong>Click to Open</strong></summary>

### شرح بسيط

HTML هي اللغة اللي بنوصف بيها محتوى صفحات الويب:
عناوين — نصوص — صور — روابط — أقسام…
هيكل وتنظيم، مش لغة برمجة.

### Example

```html
<h1>Hello World</h1>
<p>This is my first paragraph.</p>
```

### 📂 File to Open

Go to `01-HTML-Structure/index.html`

</details>

---

👉 **Section 2 — Tag vs Element vs Attribute**

<details>
<summary><strong>Click to Open</strong></summary>

### 🔹 What is a Tag?

الكلمة اللي بين `< >`

- `<p>` opening tag
- `</p>` closing tag

### 🔹 What is an Element?

التاج + المحتوى + التاج اللي بيقفل

```html
<p>Hello</p>
```

### 🔹 What is an Attribute?

معلومات إضافية جوه التاج

```html
<img src="img.jpg" alt="Photo" />
```

### مثال شامل

```html
<p class="text">Welcome to HTML</p>
```

- `tag` → p
- `element` → كل السطر
- `attribute` → class="text"

### 📂 File to Open

Go to `02-Text-Formatting/index.html` (See tags in action)

</details>

---

👉 **Section 3 — Self-Closing Tags**

<details>
<summary><strong>Click to Open</strong></summary>

### أمثلة

```html
<img src="pic.jpg" />
<br />
<hr />
```

- These tags do **not** need a closing tag like `</img>`.

### 📂 File to Open

Go to `04-Links-and-Images/index.html`

</details>

---

👉 **Section 4 — Nesting (التعشيق)**

<details>
<summary><strong>Click to Open</strong></summary>

### ✔️ صحيح

Tags must close in the reverse order they opened ("Last in, First out").

```html
<div>
  <p>Hello</p>
</div>
```

### ❌ خطأ

Don't overlap tags!

```html
<div>
  <p>Hello
</div>
</p>
```

</details>

---

👉 **Section 5 — id / class / name**

<details>
<summary><strong>Click to Open</strong></summary>

### 🔹 class

- يتكرر عادي
- نستخدمه لتجميع عناصر لها نفس التصميم
- **CSS selector**: `.className`

### 🔹 id

- فريد (مرة واحدة فقط)
- نستخدمه لاستهداف عنصر معين
- **CSS selector**: `#idName`

### 🔹 name

- خاص بالـ `input` & `forms`
- مش معمول للتصميم
- لكن ممكن أستهدفه في CSS لو احتجت `input[name="x"]`
- مهم جدًا للـ backend

### HTML Example

```html
<h1 id="main-title">HTML Session</h1>

<p class="info">Paragraph one</p>
<p class="info">Paragraph two</p>

<!-- Name attribute example -->
<input type="text" name="username" placeholder="Enter your name" />
```

### CSS Example

```css
#main-title {
  color: blue;
}

.info {
  color: green;
}

input[name="username"] {
  border: 2px solid red;
}
```

### 📂 File to Open

Go to `05-Basic-CSS/index.html`

</details>

---

👉 **Section 6 — Quick Comparison Table**

<details>
<summary><strong>Click to Open</strong></summary>

| Property  | Used for       | Repeat? | CSS Selector      |
| :-------- | :------------- | :------ | :---------------- |
| **id**    | عنصر واحد محدد | ❌ No   | `#id`             |
| **class** | مجموعة عناصر   | ✔️ Yes  | `.class`          |
| **name**  | Forms          | ✔️      | `input[name="x"]` |

</details>

---

👉 **Section 7 — Mini Exercise**

<details>
<summary><strong>Click to Open</strong></summary>

### Task

اكتب صفحة HTML بسيطة فيها:

1.  عنوان له `id`
2.  فقرتين لهم `class` واحد
3.  `input` له `name`
4.  وطبّق عليهم CSS بسيط

</details>
