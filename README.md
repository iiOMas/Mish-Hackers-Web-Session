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

**Structure Breakdown**

```
Element
   👇
 <p> Hello World </p>
  👆      👆      👆
  Tag   Content  Closing Tag
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

---

# 🟦 **HTML Page Structure — الجزء الثاني**

## 🧠 1️⃣ الهيكل الأساسي لأي صفحة HTML

كل صفحة HTML ليها **هيكل أساسي ثابت**:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Page Title</title>
  </head>
  <body>
    <!-- Content goes here -->
  </body>
</html>
```

**Explanation:**

- `<!DOCTYPE html>` → بيقول للمتصفح إن دي صفحة HTML5
- `<html>` → بداية الصفحة كلها
- `<head>` → مكان المعلومات اللي مش بتظهر على الصفحة زي العنوان، الروابط للـ CSS أو الـ meta tags
- `<title>` → عنوان الصفحة اللي بيظهر في التاب بتاع المتصفح
- `<body>` → كل حاجة المستخدم يشوفها: نصوص، صور، روابط، أزرار…

---

## 2️⃣ أهم العناصر داخل `<head>`

### **meta**

- معلومات عن الصفحة زي الترميز، الوصف، أو الكلمات المفتاحية
  **مثال:**

```html
<meta charset="UTF-8" />
```

- **ليه مهم؟**: عشان المتصفح يفهم الحروف العربي والرموز (Emojis) ويظهرها صح. من غيره الكلام ممكن يبان رموز غريبة. 😵‍💫

```html
<meta name="description" content="This is my website" />
```

### **link**

- بيربط الصفحة بـ CSS خارجي
  **مثال:**

```html
<link rel="stylesheet" href="style.css" />
```

### **script**

- لو هتستخدم JavaScript
  **مثال:**

```html
<script src="script.js"></script>
```

---

### 📂 Practical Example

Go to folder `02-HTML-Structure` to see the code in action!
