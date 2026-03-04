02 - CSS Display Property

Objective

The "display" property defines how an element is rendered in the document flow.

It controls:

- Whether an element behaves as block or inline
- Whether it generates a new formatting context
- Whether it participates in layout at all

Understanding "display" is fundamental before learning Flexbox and Grid.

---

1️⃣ Block Elements

"display: block;"

- Takes full width of its parent
- Starts on a new line
- Can have width and height

Examples:

- "div"
- "p"
- "section"
- "h1"–"h6"

div {
  display: block;
}

---

2️⃣ Inline Elements

"display: inline;"

- Does NOT start on a new line
- Takes only the width of its content
- Cannot set width and height properly
- Vertical margins behave differently

Examples:

- "span"
- "a"
- "strong"

span {
  display: inline;
}

---

3️⃣ Inline-Block

"display: inline-block;"

- Stays inline (no line break)
- Allows width and height
- Respects vertical margins

.box {
  display: inline-block;
  width: 100px;
  height: 100px;
}

Used commonly for:

- Buttons
- Cards
- Navigation items

---

4️⃣ None

"display: none;"

- Removes element completely from layout
- No space is reserved

.hidden {
  display: none;
}

Important:
This is different from "visibility: hidden;" (which hides but keeps space).

---

5️⃣ Flex

- Creates a flex formatting context
- Enables one-dimensional layout

.container {
  display: flex;
}

Flex is covered deeply in a later module.

---

6️⃣ Grid

- Creates a grid formatting context
- Two-dimensional layout

.grid {
  display: grid;
}

---

Summary Table

Display Value| New Line| Width/Height Control| Layout Type
block| Yes| Yes| Normal flow
inline| No| No (limited)| Inline flow
inline-block| No| Yes| Hybrid
none| N/A| N/A| Removed
flex| Yes| Yes| Flexbox
grid| Yes| Yes| Grid

---

Key Takeaways

- "block" = full width + new line
- "inline" = content width + no new line
- "inline-block" = best of both
- "none" = removed from DOM flow
- "flex" and "grid" = layout systems

Mastering "display" helps you understand how elements naturally behave before applying advanced layout systems.
