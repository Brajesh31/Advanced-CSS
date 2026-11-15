# 🧪 Browser Testing and Visual Review

Advanced-CSS has no automated test runner or build process. Testing is performed by opening each HTML document in a browser and reviewing the rendered result.

## 📚 Contents

- [Testing goals](#testing-goals)
- [Manual test procedure](#manual-test-procedure)
- [Task-level checks](#task-level-checks)
- [Responsive testing](#responsive-testing)
- [Accessibility checks](#accessibility-checks)
- [Screenshot review](#screenshot-review)
- [Validation before contribution](#validation-before-contribution)

## Testing goals

A useful review confirms that:
- The page opens without errors.
- Embedded CSS is applied.
- Relative assets load.
- The intended CSS behaviour is visible.
- The page remains usable at different viewport sizes.
- Keyboard and motion preferences are considered.
- The screenshot represents the expected result.

## Manual test procedure

1. Open the target task in a current browser.
2. Set browser zoom to 100%.
3. Review the page at a desktop width.
4. Resize to a tablet and narrow mobile viewport.
5. Inspect the browser console.
6. Check every image and relative path.
7. Test keyboard navigation if controls exist.
8. Compare with the task's output image.
9. Record browser and viewport details for meaningful visual changes.

## Task-level checks

| Task | Main validation |
|---|---|
| Task 1 | Both buttons render with the intended custom-property colours |
| Task 2 | Six faces form a 3D object and rotation animation is valid |
| Task 3 | Circular loader is centred and animation rotates smoothly |
| Task 4 | The referenced image loads and the visibility explanation is accurate |
| Task 5 | The output image loads and matches the intended exercise |

The repository currently has no browser automation configuration. Do not claim automated browser tests have passed unless such a test suite is added and run.

## Responsive testing

Check at least one narrow mobile, one tablet, and one desktop viewport. Inspect fixed widths, heights, transforms, overflow, and image sizing. Test the actual task rather than relying on the presence of a viewport meta tag.

## Accessibility checks

- Navigate interactive controls using only a keyboard.
- Confirm visible focus indicators.
- Check text/background contrast.
- Provide meaningful image alternative text.
- Avoid relying on colour alone.
- Emulate reduced motion.
- Ensure important status information is not conveyed only through a spinner.

## Screenshot review

Reference images are visual aids, not exact pixel-perfect test oracles. Differences can come from browser engine, operating system, device pixel ratio, zoom, fonts, or viewport dimensions.

When refreshing an output image, explain the intentional visual change in the commit or pull request.

## Validation before contribution

From the repository root, run:

```bash
git diff --check
```

Then open each changed page and verify the relevant browser behaviour. There is no npm test or build command in this static repository.
