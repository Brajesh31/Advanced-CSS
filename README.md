# 🎨 Advanced CSS Assignments

<p align="center">
  <strong>A practical collection of standalone HTML and CSS exercises.</strong>
</p>

<p align="center">
  Explore CSS custom properties, 3D transforms and perspective, keyframe animation, visibility behaviour, and visual presentation through five small browser-based tasks.
</p>

<p align="center">
  <a href="https://github.com/Brajesh31/Advanced-CSS">Repository</a> ·
  <a href="https://github.com/Brajesh31/Advanced-CSS/issues">Issues</a> ·
  <a href="docs/README.md">Documentation</a> ·
  <a href="CONTRIBUTING.md">Contributing</a>
</p>

---

## 📚 Table of Contents

1. [🌟 Project Overview](#-project-overview)
2. [🎯 Learning Objectives](#-learning-objectives)
3. [✨ Assignment Index](#-assignment-index)
4. [🧠 CSS Concepts Covered](#-css-concepts-covered)
5. [🗂️ Repository Structure](#️-repository-structure)
6. [🖥️ Requirements](#️-requirements)
7. [🚀 Getting Started](#-getting-started)
8. [▶️ Running the Exercises](#️-running-the-exercises)
9. [🧪 Reviewing the Output](#-reviewing-the-output)
10. [📱 Responsive Testing](#-responsive-testing)
11. [♿ Accessibility Checklist](#-accessibility-checklist)
12. [🛠️ Development Guidelines](#️-development-guidelines)
13. [🚀 Static Deployment](#-static-deployment)
14. [🧯 Troubleshooting](#-troubleshooting)
15. [🤝 Contributing](#-contributing)
16. [🔐 Security and Privacy](#-security-and-privacy)
17. [🗺️ Roadmap](#️-roadmap)
18. [🧩 Assignment Catalogue](#-assignment-catalogue)
19. [📖 Documentation](#-documentation)
20. [📄 License](#-license)

---

## 🌟 Project Overview

**Advanced CSS** is a learning repository containing five independent HTML pages. Each page focuses on a specific CSS task and can be opened directly in a modern web browser.

The exercises are intentionally lightweight. They do not depend on React, Node.js, a bundler, a database, or a backend API. CSS is written inside the task documents, and the `Output/` directory stores visual reference images for the assignments.

The repository is useful for practising how CSS declarations affect layout, transforms, motion, visibility, and the final appearance of browser-rendered content.

> [!NOTE]
> These are focused learning exercises, not a production design system or a complete website template. Some tasks demonstrate a concept in a minimal way and may have limitations that are worth improving as part of further practice.

## 🎯 Learning Objectives

By exploring and modifying the examples, you can practise:

- Declaring and reusing CSS custom properties.
- Applying three-dimensional transforms to HTML elements.
- Understanding perspective and transform origins.
- Creating keyframe-based animations.
- Building a simple circular loading indicator.
- Distinguishing visibility from layout removal.
- Organizing standalone HTML documents.
- Comparing browser output against reference screenshots.
- Testing layouts at different viewport sizes.
- Improving semantic HTML and accessibility.

## ✨ Assignment Index

All exercises are stored in [`Assignment_13_Advanced CSS/`](Assignment_13_Advanced%20CSS/).

| Assignment | File | Main concept | Reference |
|---|---|---|---|
| Task 1 | [Task_1.html](Assignment_13_Advanced%20CSS/Task_1.html) | CSS custom properties and `var()` | [Preview](Assignment_13_Advanced%20CSS/Output/task_1.png) |
| Task 2 | [Task_2.html](Assignment_13_Advanced%20CSS/Task_2.html) | 3D cube, perspective, transforms, animation | [Preview](Assignment_13_Advanced%20CSS/Output/task_2.png) |
| Task 3 | [Task_3.html](Assignment_13_Advanced%20CSS/Task_3.html) | Circular loader and keyframes | [Preview](Assignment_13_Advanced%20CSS/Output/task_3.png) |
| Task 4 | [Task_4.html](Assignment_13_Advanced%20CSS/Task_4.html) | Visibility behaviour demonstration | [Preview](Assignment_13_Advanced%20CSS/Output/task_4.png) |
| Task 5 | [Task_5.html](Assignment_13_Advanced%20CSS/Task_5.html) | Visual result exercise | [Preview](Assignment_13_Advanced%20CSS/Output/task_5.png) |

### 🧩 Task 1: CSS custom properties

This page explains how a CSS custom property can hold a reusable value and how the `var()` function reads it.

The example defines primary and secondary colour tokens under `:root`, then uses them to style two buttons. It illustrates how a value can be changed centrally rather than repeated across multiple selectors.

Topics to explore:
- Custom property names beginning with `--`.
- The global `:root` selector.
- The `var(--property-name)` function.
- Fallback values such as `var(--brand-color, blue)`.
- Scope and inheritance of custom properties.

### 🧊 Task 2: 3D cube

This page creates six faces and positions them in three-dimensional space. The container establishes perspective, while each face uses a transform to occupy a side of the cube. A keyframe animation rotates the object.

Topics to explore:
- `perspective` and `perspective-origin`.
- `transform-style: preserve-3d`.
- `rotateX()`, `rotateY()`, and `translateZ()`.
- Transform order.
- Keyframe animation and timing functions.
- The effect of opacity and borders on overlapping faces.

The current source is a learning example. Inspect transform values carefully when modifying it. For example, CSS angle values should be written as valid values such as `rotateX(20deg)`, without quotation marks.

### ⏳ Task 3: circular loader

This page uses a circular border with a differently coloured top edge. A continuous keyframe animation rotates the element to create a loading indicator.

Topics to explore:
- Border styling.
- Circular shapes using `border-radius: 50%`.
- Animation duration and iteration count.
- The `linear` timing function.
- The `@keyframes` rule.
- Reduced-motion preferences for users who disable animation.

### 👁️ Task 4: visibility demonstration

This page contains explanatory text and a reference image. It introduces the CSS `visibility: hidden` behaviour.

A useful distinction for further experimentation:
- `visibility: hidden` hides an element while preserving its layout space.
- `display: none` removes the element from the layout.
- `opacity: 0` makes an element transparent but does not by itself prevent interaction or keyboard focus.

Try these properties on elements inside a container and compare the space each one occupies.

### 🖼️ Task 5: visual result

This page presents a short explanation and its associated reference image. The original task is intentionally retained as a standalone exercise. Consult the screenshot and HTML together when studying or extending the result.

> [!TIP]
> Keep the original task intact when adding an improved version. A separate file makes it easier to compare the original exercise with your own implementation.

## 🧠 CSS Concepts Covered

| Concept | Why it matters | Where to explore |
|---|---|---|
| Custom properties | Reuse design values and centralize changes | Task 1 |
| Root scope | Make tokens available across the document | Task 1 |
| Fallback values | Provide a value when a custom property is missing or invalid | Task 1 extension |
| 3D perspective | Create depth in a transformed scene | Task 2 |
| 3D transforms | Position and rotate elements in three dimensions | Task 2 |
| Keyframes | Define animation states over time | Tasks 2 and 3 |
| Border styling | Build a simple visual indicator | Task 3 |
| Visibility | Understand hiding without removing layout space | Task 4 |
| Image references | Compare implementation with captured output | Tasks 4 and 5 |

## 🗂️ Repository Structure

```text
Advanced-CSS/
├── Assignment_13_Advanced CSS/
│   ├── Task_1.html
│   ├── Task_2.html
│   ├── Task_3.html
│   ├── Task_4.html
│   ├── Task_5.html
│   └── Output/
│       ├── task_1.png
│       ├── task_2.png
│       ├── task_3.png
│       ├── task_4.png
│       └── task_5.png
├── docs/
│   ├── architecture.md
│   ├── deployment.md
│   ├── development.md
│   ├── faq.md
│   ├── installation.md
│   └── troubleshooting.md
├── .editorconfig
├── .gitignore
├── CHANGELOG.md
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── LICENSE
├── README.md
├── ROADMAP.md
├── SECURITY.md
└── SUPPORT.md
```

The repository intentionally has no `package.json` or npm-based build process. Do not run `npm install` expecting a project dependency tree.

## 🖥️ Requirements

You need only:

- A modern web browser such as Chrome, Firefox, Edge, or Safari.
- A text editor or IDE for editing HTML and CSS.
- Git, if you plan to clone the repository or contribute.

Python is optional and is useful for starting a local static server.

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/Brajesh31/Advanced-CSS.git
cd Advanced-CSS
```

### 2. Open the assignment directory

The directory name contains a space, so quote it when using shell commands.

```bash
cd "Assignment_13_Advanced CSS"
```

### 3. Open a task

You can double-click any HTML file, or open it from a terminal:

```powershell
Start-Process ".\Task_1.html"
```

On macOS:

```bash
open Task_1.html
```

On Linux:

```bash
xdg-open Task_1.html
```

## ▶️ Running the Exercises

### Option A: Open files directly

Open any of the five HTML files in a browser. This is enough for the current standalone examples.

### Option B: Start a local static server

From the repository root, run:

```bash
python -m http.server 8000
```

Then visit:

```text
http://localhost:8000/Assignment_13_Advanced%20CSS/Task_1.html
```

Replace `Task_1.html` with `Task_2.html`, `Task_3.html`, `Task_4.html`, or `Task_5.html` to view another exercise.

Stop the server with `Ctrl+C`.

A local server is useful when you introduce relative assets or browser features that behave differently under a `file://` URL.

## 🧪 Reviewing the Output

Each task has a corresponding screenshot in the `Output/` folder. Use these images as visual references, not as proof that every browser will render every pixel identically.

A practical review process:

1. Open the HTML page in the target browser.
2. Set a known browser zoom level, preferably 100%.
3. Compare the page with the matching output image.
4. Check the viewport dimensions if the layout differs.
5. Inspect the browser developer tools for errors.
6. Confirm that all relative images load correctly.
7. Record intentional differences in the change description.

Screenshots should be replaced only when the expected result intentionally changes. Avoid updating reference images merely to hide a regression.

## 📱 Responsive Testing

Even small CSS exercises can overflow or behave unexpectedly at narrow widths.

Review each changed page at:
- A narrow mobile viewport.
- A typical tablet viewport.
- A desktop viewport.
- A larger display where fixed dimensions may appear too small.

Look for:
- Horizontal scrolling.
- Text overlapping controls.
- Fixed dimensions that do not shrink.
- 3D content clipping at the container edge.
- Buttons with insufficient tap targets.
- Images exceeding the viewport.
- Animations that cause unwanted motion.

Do not assume a page is responsive merely because it includes a viewport meta tag.

## ♿ Accessibility Checklist

For every exercise, consider:

- Use semantic HTML elements where they communicate meaning.
- Provide descriptive alternative text for meaningful images.
- Keep text contrast readable.
- Preserve visible keyboard focus.
- Ensure interactive controls can be reached and operated by keyboard.
- Avoid relying on colour alone to communicate meaning.
- Respect `prefers-reduced-motion` for non-essential animations.
- Avoid using animation as the only way to communicate important information.
- Give loading indicators accessible context when used in a real interface.

A purely decorative spinner may be hidden from assistive technology. A meaningful loading state should include text or an accessible status description.

## 🛠️ Development Guidelines

Keep each exercise self-contained unless there is a clear reason to introduce shared CSS or shared assets.

Recommended practices:
- Use readable, descriptive selectors.
- Prefer CSS custom properties for repeated theme values.
- Keep selectors scoped to the relevant task.
- Avoid unnecessary JavaScript and external dependencies.
- Keep HTML structure semantic and easy to inspect.
- Use consistent indentation.
- Add comments when a CSS technique is not self-explanatory.
- Test the actual browser result after every meaningful layout change.
- Preserve the original assignment and its learning objective.

### Suggested improvement workflow

1. Choose one task.
2. Identify the CSS concept being demonstrated.
3. Reproduce the current behaviour before editing.
4. Change one concept at a time.
5. Test at multiple viewport widths.
6. Compare the reference screenshot.
7. Check keyboard use and reduced motion.
8. Update the task notes or screenshot if the expected result changed.
9. Review the full Git diff before committing.

## 🚀 Static Deployment

The repository can be hosted as static files. No server-side runtime or build step is currently required.

General deployment checklist:

1. Publish the repository contents using a static hosting provider.
2. Confirm the host serves the repository root or the intended project path.
3. Test all five task URLs.
4. Confirm that image paths under `Output/` resolve correctly.
5. Test URL encoding for the directory name containing a space.
6. Enable HTTPS.
7. Confirm the deployed output matches the source commit.
8. Avoid exposing private assets or credentials.

No specific production URL or hosting provider is assumed in this guide.

## 🧯 Troubleshooting

| Problem | What to check |
|---|---|
| HTML page does not open | Confirm the path and quote the directory name with spaces |
| Output image is missing | Check relative path, filename, and case sensitivity |
| 3D cube looks flat | Inspect perspective and transform-style declarations |
| Cube faces overlap unexpectedly | Review transform order and translateZ distance |
| Animation does not run | Check keyframe name, animation declaration, and browser console |
| Layout overflows | Inspect fixed widths, viewport size, and absolute positioning |
| CSS variable is not applied | Check custom property spelling, scope, and fallback |
| Local server cannot start | Confirm Python is installed and port 8000 is available |

For more detailed help, see [docs/troubleshooting.md](docs/troubleshooting.md).

## 🤝 Contributing

Contributions that improve correctness, clarity, accessibility, responsiveness, and learning value are welcome.

Before submitting:
- Read [CONTRIBUTING.md](CONTRIBUTING.md).
- Check the existing issues and roadmap.
- Keep changes focused on the relevant exercise.
- Test the browser output.
- Describe any screenshot changes.
- Do not commit editor caches, temporary files, or private information.

## 🔐 Security and Privacy

This repository currently contains static HTML, CSS, and PNG reference images. It does not require account credentials or a backend service.

Still:
- Do not commit API keys, passwords, tokens, or private information.
- Review external links and assets before adding them.
- Avoid embedding untrusted third-party scripts.
- Do not upload screenshots containing personal or sensitive information.
- Report suspected vulnerabilities privately using [SECURITY.md](SECURITY.md).

## 🗺️ Roadmap

The roadmap tracks possible improvements such as richer task descriptions, accessible animation behaviour, responsive examples, and clearer visual references.

See [ROADMAP.md](ROADMAP.md). Roadmap entries are proposals unless explicitly marked as completed.

## 🧩 Assignment Catalogue

For detailed task-by-task explanations and guided experiments, see [TASKS.md](TASKS.md).

## 📖 Documentation

| Document | Description |
|---|---|
| [Installation](docs/installation.md) | Open the examples and start a local server |
| [Architecture](docs/architecture.md) | Understand the static repository structure |
| [CSS Technique Reference](docs/css-reference.md) | Review custom properties, 3D transforms, motion, and visibility |
| [Accessibility](docs/accessibility.md) | Improve keyboard, contrast, image, and motion support |
| [Testing](docs/testing.md) | Manual browser and screenshot review |
| [Development](docs/development.md) | Modify and validate exercises |
| [FAQ](docs/faq.md) | Common questions |
| [Troubleshooting](docs/troubleshooting.md) | Diagnose common problems |
| [Deployment](docs/deployment.md) | Publish the static exercises |
| [API](docs/api.md) | Repository API scope |
| [Database](docs/database.md) | Database scope and current absence |
| [Contributing](CONTRIBUTING.md) | Contribution expectations |
| [Security](SECURITY.md) | Responsible security reporting |
| [Code of Conduct](CODE_OF_CONDUCT.md) | Community expectations |
| [Support](SUPPORT.md) | Help and issue reporting |
| [Changelog](CHANGELOG.md) | Verified project history |

## 📄 License

This repository is distributed under the MIT License. See [LICENSE](LICENSE) for the full text.

---

**Maintained by Brajesh Kumar** · [GitHub](https://github.com/Brajesh31)

Last updated: 2026-11-15 20:17 UTC
