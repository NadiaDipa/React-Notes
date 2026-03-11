# JSX (JavaScript XML)

**Definition:**
JSX = **JavaScript + HTML এর মতো syntax**। React এ UI বানানোর জন্য use করা হয়।


---

## 1️⃣ One Parent Element

**Explanation:** JSX এ একবারে multiple element return করতে গেলে **একটা parent element** লাগবে।
**Example:**

```jsx
// ❌ Wrong
<h1>Hello</h1>
<p>World</p>

// ✔ Correct
<div>
  <h1>Hello</h1>
  <p>World</p>
</div>
```

**Fragment:** extra `<div>` ছাড়া multiple elements return করতে দেয়।

```jsx
<>
  <h1>Hello</h1>
  <p>World</p>
</>
```

---

## 2️⃣ JavaScript Expression

**Explanation:** JSX এর ভিতরে `{}` দিয়ে JS ব্যবহার করা যায়।
**Example:**

```jsx
const name = "Diya";
<p>Hello {name}!</p>  // Output: Hello Diya
<p>{5 + 3}</p>        // Output: 8
```

---

## 3️⃣ class → className

**Explanation:** HTML এর `class` React JSX এ `className` হয়।
**Example:**

```jsx
<div className="card">Card Content</div>
```

---

## 4️⃣ Self Closing Tags

**Explanation:** HTML এর কিছু tag self-closing হয়। JSX এও same।
**Example:**

```jsx
<img src="logo.png" />
<br />
<input type="text" />
```

---

## 5️⃣ Inline CSS

**Explanation:** JSX এ style **object** আকারে লিখতে হয়।
**Example:**

```jsx
<h1 style={{ color: "blue", fontSize: "20px" }}>Hello</h1>
```

---

## 6️⃣ Component Return JSX

**Explanation:** Component UI return করার জন্য JSX use করে।
**Example:**

```jsx
function Card() {
  return <div>Card</div>;
}

// Render
<Card />
<Card />
```

---

## 7️⃣ Short Summary

* JSX = **HTML-like JavaScript**
* Rules:

  1. One parent element / Fragment
  2. JS inside `{ }`
  3. `className` instead of `class`
  4. Self-closing tags
  5. Inline CSS → object
  6. Component return → JSX

💡 **Tip:** JSX compile হয় JS এ → React can understand & render UI faster.
