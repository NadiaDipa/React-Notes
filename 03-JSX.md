# JSX (JavaScript XML)

👉 JSX = JavaScript + HTML syntax for UI in React.



---

## 1️⃣ One Parent Element

👉 In JSX, multiple elements must be inside a **single parent**.

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

👉 Return multiple elements without extra `<div>`

```jsx
<>
  <h1>Hello</h1>
  <p>World</p>
</>
```

---

## 2️⃣ JavaScript Expression

👉 Use `{}` in JSX to insert JavaScript.

**Example:**

```jsx
const name = "Diya";
<p>Hello {name}!</p>  // Output: Hello Diya
<p>{5 + 3}</p>        // Output: 8
```

---

## 3️⃣ class → className 

👉 In JSX, class becomes `className`.

**Example:**

```jsx
<div className="card">Card Content</div>
```

---

## 4️⃣ Self Closing Tags 

👉 JSX supports `self‑closing tags(<img />)`, same as HTML.

**Example:**

```jsx
<img src="logo.png" />
<br />
<input type="text" />
```

---

## 5️⃣ Inline CSS

👉 In JSX, style is written as an `object{{color: "red"}}`.

**Example:**

```jsx
<h1 style={{ color: "blue", fontSize: "20px" }}>Hello</h1>
```

---

## 6️⃣ Component Return JSX

👉 JSX starts after `return with <div> ... </div>`, which defines the component UI.

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

* JSX = **Combined of HTML and JavaScript**

* Rules:

  1. One parent element / Fragment
  2. JS inside `{ }`
  3. `className` instead of `class`
  4. Self-closing tags
  5. Inline CSS → object
  6. Component return → JSX

💡 **Tip:** JSX compile হয় JS এ → React can understand & render UI faster.
