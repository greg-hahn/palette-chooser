# AestheticGen // Palette & Font Pairings

**AestheticGen** is a lightweight, browser-based design companion that helps you discover, visualize, and export cohesive color palettes and typography pairings. Unlike traditional palette generators, it features a **Practical Preview**—a live mock UI that shows exactly how your choices will look on buttons, cards, and navigation elements.

## 🚀 Features

* **Dynamic Generation:** Generate cohesive 5-color palettes based on a seed hue and adjustable saturation.
* **Curated Typography:** Automatically pairs professional Google Fonts (Heading + Body) with your colors.
* **Live UI Mockup:** Real-time preview of your aesthetic applied to a dashboard-style component.
* **Accessibility First:** Integrated WCAG contrast ratio checking for White and Black text on every color swatch.
* **Saved Library:** Save your favorite combinations to your browser’s `localStorage` for future sessions.
* **Developer Exports:** Copy CSS variables or JSON objects with a single click.
* **Themed Interface:** Built-in Dark and Light modes for the application itself.

---

## ⌨️ Keyboard Shortcuts

Speed up your workflow with native hotkeys:

| Key | Action |
| :--- | :--- |
| **Space** | Shuffle new palette and font pairing |
| **S** | Save current combo to Library |
| **C** | Copy Palette as CSS Variables |
| **J** | Export current state as JSON |

---

## 🛠️ Technical Stack

This project is built with **Vanilla Web Technologies**—no frameworks or heavy dependencies required.

* **HTML5 & CSS3:** Utilizes CSS Custom Properties (Variables) for the theme engine and mock UI.
* **Vanilla JavaScript:**
    * **Color Logic:** Custom HSL-to-HEX conversion and hue-shifting algorithms.
    * **Accessibility:** Luminance-based contrast ratio calculation ($L1 / L2$ formula).
    * **Storage:** Persistent state via the Web Storage API.
* **Google Fonts API:** Dynamic loading of font weights and styles.

---

## 📂 Installation & Usage

Since AestheticGen is a client-side application, no installation is necessary.

1.  Clone the repository or download the `index.html` file.
2.  Open `index.html` in any modern web browser.
3.  Adjust the **Base Color** and **Saturation** to influence the generation logic.
4.  Hit **Shuffle** or press `Space` until you find a look you love.

---

## 🧪 Palette Logic

The generator uses a seed color to create a balanced UI system:
1.  **Dark:** Deeply desaturated variant for text.
2.  **Light/BG:** High-luminance variant for backgrounds.
3.  **Primary:** The core brand color.
4.  **Secondary:** A 30° hue-shifted companion.