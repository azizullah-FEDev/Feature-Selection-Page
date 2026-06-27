# Feature Selection Page

A clean and interactive feature selection UI built with pure HTML and CSS. Users can browse available features and select them using styled checkboxes — no JavaScript required.

---

## Project Structure

```
project/
├── index.html       # Main HTML page
├── styles.css       # All styling and checkbox logic
└── README.md        # Project documentation
```

---

## Features

- 6 selectable feature cards displayed in a responsive layout
- Custom styled checkboxes with gold/yellow color theme
- Hover effects with orange glow on cards
- Checked state shows a gold background with a ✓ checkmark
- Fully built with HTML and CSS only — no JavaScript

---

## Feature Cards Included

| Feature | Description |
|---|---|
| Cloud Storage | 100 Gigabyte secure storage |
| Dedicated Support | 24/7 customer help support |
| Advanced Analytics | Insights & reports |
| Custom User Themes | Personalized dashboard design |
| Multi-User Collab | Team access and sharing |
| API Access | Integrate with your custom tools |

---

## How It Works

### HTML (`index.html`)
- Each card is a `<label>` element wrapping an `<input type="checkbox">`
- Using `<label>` means clicking anywhere on the card toggles the checkbox
- All cards sit inside a `.feature-card-container` div

### CSS (`styles.css`)

**Card Layout:**
```css
.feature-card-container {
  display: flex;
  flex-wrap: wrap;       /* cards wrap to next row */
  justify-content: center;
  max-width: 800px;
  margin: 0 auto;
}
```

**Card Style:**
```css
.feature-card {
  display: inline-block;
  border: 2px solid #ccc;
  border-radius: 10px;
  padding: 20px;
  cursor: pointer;
  position: relative;   /* needed for checkbox positioning */
}
```

**Hover Effect:**
```css
.feature-card:hover {
  border-color: #FFBF00;
  box-shadow: 0 4px 8px rgba(255, 142, 4, 0.685);
}
```

**Custom Checkbox:**
```css
input[type="checkbox"] {
  appearance: none;          /* removes default browser style */
  border: 2px solid #FFBF00;
  background-color: white;
  border-radius: 4px;
}

input[type="checkbox"]:checked {
  background-color: #FFBF00; /* gold fill when checked */
}

input[type="checkbox"]:checked::after {
  content: "✓";              /* checkmark appears */
  color: white;
}
```

---

## Color Theme

| Usage | Color |
|---|---|
| Primary accent | `#FFBF00` (Gold/Amber) |
| Hover border | `#FFBF00` |
| Hover shadow | `rgba(255, 142, 4, 0.685)` |
| Default border | `#ccc` (Light grey) |
| Checkmark color | `white` |

---

## How to Run

1. Download or clone the project files
2. Make sure `index.html` and `styles.css` are in the **same folder**
3. Open `index.html` in any web browser
4. Click on any card to select/deselect it
