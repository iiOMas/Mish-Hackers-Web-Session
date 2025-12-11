# HTML Basics Session

## 🧠 1️⃣ HTML يعني إيه؟

-\* **HTML** = لغة لوصف محتوى صفحات الويب.

- **استخداماتها**: العناوين، النصوص، الروابط، القوائم.
- **مش لغة برمجة**: دي لغة ترتيب وهيكل.

### 💡 Analogy: Start with MS Word

Think of HTML like a Word Document.
When you write in Word, you choose:

- **Big Title** (Heading 1)
- **Subtitle** (Heading 2)
- **Paragraph text**
- **Bold/Italic**

HTML does the EXACT same thing, but with code.

![Word Structure Analogy](images/word-structure.png)

### Example

```html
<h1>Hello World</h1>
{{ ... }}
```

---

## 2️⃣ Tag / Element / Attribute

### 🔹 Tag

كلمة بتتكتب بين علامات `< >`:

- **Open Tag**: `<p>` (البداية)
- **Close Tag**: `</p>` (النهاية)

### 🔹 Element

هو "العنصر الكامل": (البداية + المحتوى + النهاية).

**Visual Breakdown** 👇

```html
Element ┌───────┐
<p>Hello</p>
👆 👆 👆 Tag Content Closing
```

### Attribute

معلومة صغيرة جوه التاج بتحدد خصائص العنصر.
شكلها: `name="value"`

### Example Attributes

```html
<a href="https://google.com" target="_blank">Google</a>
<p class="text">Hello!</p>
<input type="text" name="username" placeholder="Enter your name" />
```

---

## 3️⃣ Self-Closing Tags

بعض العناصر **ملهاش محتوى جوه** → مش محتاجة تاج إغلاق.

```html
<br />
<hr />
```

---

## 4️⃣ id / class / name

### class

- لتكرار الشكل على أكتر من عنصر
- CSS Selector: `.className`

### id

- فريد لعنصر واحد
- CSS Selector: `#idName`

### name

- غالبًا في الفورمز
- CSS ممكن نستهدفه بـ `[name="value"]`

### Example HTML + CSS

```html
<h1 id="main-title">Welcome to the page</h1>
<p class="info">Paragraph 1</p>
<p class="info">Paragraph 2</p>
<input type="text" name="username" placeholder="Enter your name" />
```

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

### 📂 Practical Example

Go to folder `01-HTML-Basics` to see the code in action!
