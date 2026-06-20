# Flarum AMOLED Purple Overhaul

A modern, high-performance custom CSS theme for Flarum forums developed by ElysianNodes. Built with a deep AMOLED black background, vibrant electric purple accents, squircle components, and native glassmorphism effects. 

This layout is fully optimized to be Less-safe, avoiding standard CSS variable function issues that break the Flarum preprocessor, and it uses no external dependencies or `@import` declarations.
Demo: https://forums.jimi.lol/
---

## Features

* **AMOLED Black Foundation:** Uses deep blacks (`#050508`) to maximize contrast and reduce eye strain.
* **Electric Purple Branding:** Consistent accent structure, active state markers, and hover indicators using a purple color palette.
* **Squircle Elements:** Modifies generic round avatar and icon elements into a uniform rounded-corner layout.
* **Glassmorphic Navigation Header:** Implements modern `backdrop-filter` rules to blend elements cleanly during page scroll.
* **No External Dependencies:** Fully localized stylesheet with zero external assets or `@import` calls.
* **Less Compiler Integration:** Uses native `color-mix()` syntax to bypass asset pipeline calculation errors during saving.

---

## Installation Guide

No terminal or system-level directory changes are required. The theme can be added entirely through your administration dashboard.

### 1. Locate the Stylesheet
All custom CSS rules are maintained within the `style.css` file included in this repository. Open the file and copy its entire contents to your clipboard.

### 2. Apply Changes
1. Navigate to your Flarum Admin Dashboard.
2. Select the **Appearance** section from the sidebar layout.
3. Locate the text field labeled **Custom Styles**.
4. Paste the copied CSS configuration from `style.css` directly into the input container.
5. Click **Save Changes** to finish the integration.

---

## Variable Customization

The design theme uses standard CSS root variables. Modifying target hex values or branding ranges can be handled directly at the top of the `style.css` file under the `:root` pseudo-class.

```css
:root {
  /* System Background Configuration */
  --bg-amoled: #000000; /* Pure black target scaling */
  --bg-card: #0a0a0f;   /* Discussion listing component background */
  
  /* Accent Branding Configuration */
  --purple-primary: #a855f7; /* Primary accent configuration */
  --purple-glow: #c084fc;    /* Secondary text link configuration */
}
