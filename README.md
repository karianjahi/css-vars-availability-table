# css-vars-availability-table

A lightweight, responsive HTML/CSS project that demonstrates the use of CSS custom properties (variables) to build a visual weekly availability table.

## 📌 Purpose

This project is a visual demonstration of how to effectively use **CSS custom properties** (a.k.a. CSS variables) to build scalable and themeable UIs. The central feature is a weekly **availability heatmap table** styled using reusable and semantic variables.

---

## 🧠 Features

- 📅 Weekly schedule table (Monday to Sunday, hourly blocks)
- 🎨 CSS custom properties for color theming and layout
- 🟢 Gradient legend indicating availability scale
- ✍️ Clean and accessible HTML structure
- 🔍 Easy to extend for different use cases (e.g., booking systems, shift planning)

---

---

## 💡 How It Works

### 1. **Semantic Class Naming**
Each cell in the table uses a class like `.available-0` to `.available-5`, corresponding to the degree of availability.

### 2. **CSS Custom Properties**
Defined in the `:root` selector to support easy theme updates:

```
:root {
  --color0: #f4f8f5;
  --color1: #74bd8c;
  --color2: #36834f;
  --color3: #16552b;
  --color4: #09411c;
  --color5: #043317;
  --solid-border: solid;
  --dashed-border: dashed;
  --table-border-color: #000505;
}
```

### 3. Heatmap Table
The table uses the classes to apply background colors based on availability levels:
```
    .available-0 { background-color: var(--color0); }
    .available-1 { background-color: var(--color1); }
    /* ... up to .available-5 */

```

### 4. Legend
The gradient legend helps users visually decode the meaning of the availability colors.

## 📚 Concepts Illustrated
- CSS Variables (--var)

- Table styling with borders

- Semantic class naming conventions

- Linear gradients

- Responsive layout using viewport units (vh, vw)


 ## License
This project is licensed under the MIT License.