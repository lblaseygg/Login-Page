# Practice Login with Dark/Light Mode

This project is a simple practice login page that includes styled input fields, a button, and a toggle switch to switch between **Dark Mode** and **Light Mode** using HTML, CSS, and JavaScript.

---

## Features

- **HTML**: Structuring of the login form and related elements.
- **CSS**: Styled components for an aesthetically pleasing login page.
- **Dark/Light Mode Toggle**: A JavaScript-powered switch to dynamically toggle the page's theme.

---

## Technologies Used

1. **HTML**: For structuring the webpage.
2. **CSS**: To style the elements (e.g., colors, margins, buttons).
3. **JavaScript**: For implementing the dark/light mode toggle functionality.

---

## File Structure

```
project-folder/
|-- index.html       # The main HTML file
|-- style.css        # CSS file for styling
|-- script.js        # JavaScript file for functionality
|-- README.md        # Documentation (this file)
```

---

## Dark/Light Mode Implementation

The Dark/Light mode switch uses JavaScript to toggle themes dynamically by manipulating a `data-theme` attribute on the `body` element:

1. **Switch Structure**: The switch is implemented using an HTML checkbox element.
2. **JavaScript**: When the switch is toggled:
   - A `data-theme="dark"` attribute is added to or removed from the body tag.
   - CSS custom properties (variables) are used to define light and dark mode styles.

---

## Usage

1. Clone or download the repository.
2. Open `index.html` in a browser to view the page.
3. Interact with the toggle switch to see the theme change dynamically.

---

## Example Code Snippets

### **HTML** (Toggle Switch)
```html
<label class="theme-switch">
    <input type="checkbox" onclick="toggleTheme()">
    <span class="slider"></span>
</label>
```

### **CSS** (Dark Mode Styles)
```css
[data-theme="dark"] {
    --bg-color: #1a1a1a;
    --text-color: #ffffff;
    --input-bg: #333333;
    --box-shadow: 0 4px 6px rgba(0, 0, 0, 0.3);
}
```

### **JavaScript** (Toggling Theme)
```javascript
function toggleTheme() {
    const body = document.body;
    if (body.getAttribute('data-theme') === 'dark') {
        body.removeAttribute('data-theme');
    } else {
        body.setAttribute('data-theme', 'dark');
    }
}
```

---

## Future Enhancements

- Add animations for a smoother theme transition.
- Store the user's theme preference in local storage.

---

## Author

Created by Luis Feliciano as part of a practice project exploring basic web development concepts.

