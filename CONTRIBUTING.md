# 🤝 Contributing to Advanced CSS

Thank you for helping improve this collection of HTML and CSS exercises. Contributions should make the examples more accurate, easier to understand, more accessible, and more useful for learners.

## 📚 Table of Contents

- [Project Scope](#-project-scope)
- [Ways to Contribute](#-ways-to-contribute)
- [Before You Start](#-before-you-start)
- [Development Workflow](#-development-workflow)
- [HTML and CSS Standards](#-html-and-css-standards)
- [Assignment Guidelines](#-assignment-guidelines)
- [Reference Screenshot Rules](#-reference-screenshot-rules)
- [Accessibility Expectations](#-accessibility-expectations)
- [Validation Checklist](#-validation-checklist)
- [Commit and Pull Request Guidelines](#-commit-and-pull-request-guidelines)

## 🎯 Project Scope

The repository currently contains five standalone HTML pages with embedded CSS and five corresponding reference images. There is no package manager or application build system.

Do not introduce a framework, bundler, runtime server, or external dependency merely to solve a small CSS exercise. Such changes need a clear learning or maintenance justification.

## 💡 Ways to Contribute

| Area | Useful contribution |
|---|---|
| Correctness | Fix invalid CSS or misleading explanation |
| Learning value | Explain why a property behaves a certain way |
| Accessibility | Improve semantics, focus, contrast, and reduced motion |
| Responsiveness | Prevent overflow and clipping at smaller widths |
| Documentation | Add examples and task-specific notes |
| Visual review | Refresh a screenshot after an intentional result change |
| Maintenance | Improve file organization without unnecessary complexity |

## 🔎 Before You Start

1. Read the root README and [TASKS.md](TASKS.md).
2. Identify the exact task and CSS concept involved.
3. Check open issues and the [roadmap](ROADMAP.md).
4. Confirm whether the change should affect the original exercise or be a separate extension.
5. Keep the original learning objective intact.

## 🛠️ Development Workflow

1. Fork or clone the repository.
2. Create a focused branch.
3. Open the target HTML file in a browser.
4. Inspect the current result before editing.
5. Make a small, isolated change.
6. Refresh the browser and inspect the result.
7. Test a narrow and wide viewport.
8. Compare the corresponding output image.
9. Run `git diff --check`.
10. Review the final diff before submitting.

No npm installation is required for the current project.

## 🧱 HTML and CSS Standards

- Use a valid document structure and include a viewport meta tag.
- Prefer semantic HTML elements.
- Use descriptive class names.
- Keep CSS readable and scoped to the task.
- Avoid unnecessary IDs for styling when classes are more appropriate.
- Use CSS custom properties for genuinely reused values.
- Use valid CSS values and avoid quoting numeric angle values.
- Keep selectors understandable for beginners.
- Add comments when a technique is difficult to infer.
- Avoid unnecessary JavaScript.
- Do not add third-party assets without checking their terms and security.

## 🧩 Assignment Guidelines

Each task should remain independently openable. Shared files are acceptable only when the benefit is clear and all affected task paths remain understandable.

When adding a task:
- Give it a descriptive title.
- Explain the concept in the HTML or task catalogue.
- Keep layout and styles easy to inspect.
- Add a corresponding output screenshot when appropriate.
- Link the task from README and TASKS.md.
- Add a manual test note.

## 🖼️ Reference Screenshot Rules

Reference images should match the expected browser output. Update an image only when the visible result intentionally changes.

When updating screenshots:
- Capture the correct task.
- Use a known viewport size.
- Keep the image legible.
- Do not crop out layout defects.
- Avoid including private browser data or personal information.
- Explain why the reference image changed.

## ♿ Accessibility Expectations

- Preserve keyboard access and visible focus.
- Use meaningful alternative text for informative images.
- Maintain readable contrast.
- Avoid relying on colour alone.
- Respect reduced-motion preferences.
- Ensure hidden elements do not create confusing focus stops.
- Keep zoom and text resizing usable.

## ✅ Validation Checklist

- [ ] The HTML page opens in a modern browser.
- [ ] No relevant browser console errors appear.
- [ ] CSS declarations are valid.
- [ ] Images and relative paths resolve.
- [ ] The page works at narrow and wide widths.
- [ ] Keyboard and focus behaviour are understandable.
- [ ] Motion preferences are respected.
- [ ] Reference screenshot is updated only when necessary.
- [ ] Documentation reflects the implementation.
- [ ] `git diff --check` passes.

## 📝 Commit and Pull Request Guidelines

Use clear commit messages such as:
- `fix: correct cube transform angle syntax`
- `docs: explain css custom property fallback`
- `feat: add responsive loader example`
- `a11y: respect reduced motion preference`

A pull request should include:
- The task changed.
- The CSS concept affected.
- The reason for the change.
- Browser and viewport used for testing.
- A screenshot when the visual result changes.
- Accessibility considerations and known limitations.
