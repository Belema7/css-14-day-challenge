01 - CSS Selectors (Core Concepts)

Objective

Selectors define which elements receive styles.

If "display" controls how elements behave,
selectors control what gets styled.

This module focuses only on the most commonly used selectors in real-world projects.

---

1️⃣ Type Selector (Element Selector)

Targets elements by tag name.

p {
  color: blue;
}

Used for:

- Global resets
- Basic typography styling

---

2️⃣ Class Selector (Most Common)

Targets elements with a class attribute.

.card {
  background: lightgray;
}

- Reusable
- Preferred over ID in most projects
- Core selector in modern CSS architecture

You will use this constantly.

---

3️⃣ ID Selector (Rarely Used in Modern CSS)

Targets an element with a unique ID.

#header {
  background: black;
}

- High specificity
- Hard to override
- Usually avoided for styling (better for JS targeting)

---

4️⃣ Descendant Selector (Very Common)

Targets elements inside another element.

.card p {
  color: red;
}

Meaning:
Select all "p" elements inside ".card".

Used frequently for scoped styling.

---

5️⃣ Child Selector

Targets only direct children.

.nav > li {
  list-style: none;
}

Important when controlling layout structure.

---

6️⃣ Grouping Selector

Apply same style to multiple selectors.

h1, h2, h3 {
  font-family: sans-serif;
}

Reduces repetition.

---

7️⃣ Pseudo-Class (State Based)

Common ones:

:hover
:focus
:first-child
:last-child

Example:

button:hover {
  background: black;
  color: white;
}

Used constantly for:

- Interactions
- UI feedback
- Lists styling

---

8️⃣ Basic Attribute Selector

Frequently used for forms and links.

input[type="text"]
a[target="_blank"]

Useful for:

- Form customization
- Targeting specific link behavior

---

Specificity (Critical)

Priority order (Low → High):

1. Type
2. Class / Attribute / Pseudo-class
3. ID
4. Inline styles

Example conflict:

p { color: blue; }
.card p { color: red; }

".card p" wins (higher specificity).

---

Real-World Rule

In modern development:

- Use classes for almost everything
- Avoid IDs for styling
- Use descendant selectors carefully (avoid deep nesting)
- Keep specificity low and predictable

---

Deliverable

You should be able to:

- Target elements precisely
- Control specificity
- Write scalable selectors
- Avoid overcomplicated chains

Selectors are about control and precision.
Master them before moving to layout systems.