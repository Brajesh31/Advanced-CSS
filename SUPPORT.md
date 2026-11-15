# 🧭 Advanced CSS Support Guide

This guide helps users run the five static HTML/CSS exercises, understand common browser issues, and report reproducible problems.

## 📚 Table of Contents

- [Start Here](#-start-here)
- [Choose a Support Path](#-choose-a-support-path)
- [Opening the Exercises](#-opening-the-exercises)
- [Task-Specific Help](#-task-specific-help)
- [Browser and Screenshot Issues](#-browser-and-screenshot-issues)
- [How to Report a Problem](#-how-to-report-a-problem)
- [What Not to Share](#-what-not-to-share)

## 🚦 Start Here

Read the [README](README.md) for the project overview, [TASKS.md](TASKS.md) for task-level guidance, and the [documentation index](docs/README.md) for technical notes.

## 🧭 Choose a Support Path

| Need | Where to go |
|---|---|
| Cannot open an HTML file | [Installation guide](docs/installation.md) |
| CSS behaviour is unclear | [CSS reference](docs/css-reference.md) |
| Need task-specific context | [Task catalogue](TASKS.md) |
| Visual result differs | [Troubleshooting](docs/troubleshooting.md) |
| Want to improve an example | [Contributing](CONTRIBUTING.md) |
| Suspect a security problem | [Security policy](SECURITY.md) |
| Have a general question | GitHub issue with a clear question |

Search existing issues before creating a new one.

## 🖥️ Opening the Exercises

No Node.js installation or package installation is required. Open an HTML page directly in a browser, or run:

```bash
python -m http.server 8000
```

from the repository root. The task pages live under `Assignment_13_Advanced CSS/`.

## 🧩 Task-Specific Help

- **Task 1:** verify custom property spelling and scope.
- **Task 2:** inspect perspective, transform order, 3D style, and angle syntax.
- **Task 3:** verify the keyframe name and animation declaration.
- **Task 4:** compare the intended visibility property with its layout effect.
- **Task 5:** check the relative screenshot path and image filename.

## 🖼️ Browser and Screenshot Issues

When output differs, verify browser zoom, viewport dimensions, device pixel ratio, font availability, relative asset paths, and browser engine. A screenshot is a reference, not a guarantee of pixel-identical output everywhere.

## 🐛 How to Report a Problem

Include:
- Task filename.
- Browser and operating system.
- Viewport dimensions.
- Steps to reproduce.
- Expected and actual behaviour.
- Relevant console message.
- Screenshot when it helps explain the issue.

A minimal example is better than a vague description.

## 🔒 What Not to Share

Do not post private information, passwords, access tokens, or screenshots that reveal personal data. Do not include unrelated credentials or machine-specific configuration in issue reports.
