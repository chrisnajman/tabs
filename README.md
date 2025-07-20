# Tabs

A fully accessible, keyboard-navigable tab interface with responsive layout, built with semantic HTML, ARIA roles, and JavaScript.

[View on GitPage](https://chrisnajman.github.io/tabs)

---

## JavaScript

Built with **vanilla ES6 JavaScript**, focusing on modern syntax and browser APIs, , then bundled, transpiled to ES2015, and minified for broad browser compatibility.

The JavaScript has been split into separate modules, improving code modularity:

### Main

- `tabs.js`: Handles the tabbed interface (selection, panel switching).
- `reset-all-tab-panels.js`: Hides all tab panels.
- `reset-all-tabs.js`: Deselects all tabs.

### Helpers

- `set-multiple-attributes.js`: Utility function to efficiently assign multiple attributes to a single DOM element.

### Other

- `loader.js`: Displays a loader animation until the page is fully rendered, then removes the loader and announces readiness for screen readers.
- `theme.js`: Handles theme toggling (light/dark mode) and local storage management.

---

## Accessibility

The site includes the following accessibility enhancements:

- Fully keyboard-navigable using tab keys and arrow keys.
- ARIA roles and attributes are implemented throughout (e.g. for tabs and panels).
- A visually hidden skip link is provided for screen reader users.

---

## Theme Toggling

The application includes a dark mode and light mode toggle:

- The current theme state is stored in **local storage** and applied automatically on page reload.
- Accessible buttons with appropriate ARIA attributes are used to improve usability.

---

## Testing and Compatibility

The application has been tested on the following platforms and browsers:

- **Operating System**: Windows 10
- **Browsers**:
  - Google Chrome
  - Mozilla Firefox
  - Microsoft Edge

### Device View Testing

The layout and functionality have been verified in both browser and device simulation views to ensure responsiveness and usability.

---

## How to Run

1. Clone or download the repository to your local machine.
2. Open the project folder and start a simple HTTP server (e.g., using `Live Server` in VS Code or Python's `http.server` module).
3. Open the project in a modern browser (e.g., Chrome, Firefox, or Edge).

---

## Build & Deployment Setup for `/docs` Folder

If you want to deploy a minified version of this project to **GitHub Pages**, read on.

### 1. Install Required Packages

Run this once in your project root to install dev dependencies:

```bash
npm install
```

### 2. Run the full build process

In the terminal, run:

```bash
npm run build
```

### 3. Deploy to GitHub Pages

Once you've created a repository and pushed the files,

- go to `https://github.com/[your-name]/[your-project-name]/settings/pages`.
- Under "Build and deployment > Branch" make sure you set the branch to `main` and folder to `/docs`.
- Click "Save".

> [!NOTE]
> For a detailed description of the build process, configuration files and npm packages see my [GitHub Pages Optimised Build](https://github.com/chrisnajman/github-pages-optimised-build).
