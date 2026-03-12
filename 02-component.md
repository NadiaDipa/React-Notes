## Components & Render

**Component →** Reusable pieces of UI...
such as **Card, Navbar, Button, Footer**.

**Render →** Calling or using a component inside the UI.

### Example

```javascript
function Card(){
  return <div>Card</div>
}
```

### Render (Using the component)

```jsx 
// render card component

<Card></Card>
<Card></Card>
<Card></Card>
```

### Diagram

```
        App
         |
   ----------------
   |      |      |
 <Card/> <Card/> <Card/>   ← render anywhere
```

👉 A component can be **written once and rendered multiple times**, similar to **calling a function**.

👉 Use **capital letters for component names**, when rendering.  
- Example: `function Card(){...}` → `<Card />`



