# Advanced CSS Assignments

This repository contains a collection of standalone HTML exercises demonstrating advanced CSS layout, positioning, visual effects, and responsive presentation techniques.

## Contents

The examples are located in [`Assignment_13_Advanced CSS`](Assignment_13_Advanced%20CSS):

- `Task_1.html`
- `Task_2.html`
- `Task_3.html`
- `Task_4.html`
- `Task_5.html`
- `Output/` contains captured output images for the exercises.

## Run the examples

No build system or package installation is required. Open any HTML file directly in a browser:

```powershell
Start-Process ".\Assignment_13_Advanced CSS\Task_1.html"
```

Alternatively, serve the repository with a local static server so relative assets behave consistently:

```powershell
py -m http.server 8000
```

Then open `http://localhost:8000/Assignment_13_Advanced%20CSS/Task_1.html`.

## Development guidance

Keep each exercise self-contained unless a shared stylesheet is deliberately introduced. Test layouts at narrow and wide viewport sizes, use semantic HTML where practical, and preserve readable contrast and keyboard focus visibility.

When changing a task, update its corresponding output image only when the captured result is intentionally changed. Avoid committing editor metadata or generated temporary files.

## Ownership and license

This repository is maintained by Brajesh Kumar (`brajesh31`). See [LICENSE](LICENSE) for the software license and review dataset or asset terms separately if additional media is introduced.

Last updated: 2026-10-17 11:49 UTC
