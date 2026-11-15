# 🧩 Assignment Catalogue

This catalogue describes the five existing Advanced CSS exercises. The goal is to help learners understand what each page demonstrates and how to extend it without losing the original learning objective.

## 📚 Contents

- [Task 1: CSS custom properties](#task-1-css-custom-properties)
- [Task 2: Three-dimensional cube](#task-2-three-dimensional-cube)
- [Task 3: Circular loader](#task-3-circular-loader)
- [Task 4: Visibility demonstration](#task-4-visibility-demonstration)
- [Task 5: Visual output exercise](#task-5-visual-output-exercise)
- [Working with output images](#working-with-output-images)
- [Suggested experiments](#suggested-experiments)

## Task 1: CSS custom properties

**File:** `Assignment_13_Advanced CSS/Task_1.html`

The page explains the purpose of the `var()` function and defines reusable colour values on `:root`. Two buttons use the primary and secondary colour tokens.

### Concepts

- CSS custom property declaration with a `--name`.
- Root-level scope.
- Reading a custom property using `var()`.
- Reusing colour values.
- Fallback values and inheritance as follow-up topics.

### Experiments

1. Change the primary colour once and observe both the declaration and rendered button.
2. Rename a custom property and update its references.
3. Add a fallback value to `var()`.
4. Define a property on a container instead of `:root`, then inspect inheritance.

## Task 2: Three-dimensional cube

**File:** `Assignment_13_Advanced CSS/Task_2.html`

The page creates six faces and places them around a centre using 3D transforms. A perspective container creates the sense of depth, and keyframes animate rotation.

### Concepts

- Perspective and viewing depth.
- `transform-style: preserve-3d`.
- Rotation around X and Y axes.
- Translation along Z.
- Transform order.
- Keyframe animation.

### Experiments

1. Change the perspective distance and observe the depth.
2. Change face size and matching `translateZ()` distances.
3. Compare `preserve-3d` with the default flat transform style.
4. Add a reduced-motion alternative.
5. Correct invalid or quoted angle values before experimenting with rotation.

## Task 3: Circular loader

**File:** `Assignment_13_Advanced CSS/Task_3.html`

A circular border with a coloured top edge is rotated continuously through a keyframe animation.

### Concepts

- Border and border-radius.
- Flex alignment.
- `@keyframes`.
- Animation duration, iteration count, and timing function.
- Motion preferences.

### Experiments

1. Change the border thickness.
2. Change the animation duration.
3. Use a different timing function.
4. Add a visible loading label for a realistic interface.
5. Use `prefers-reduced-motion` to reduce continuous motion.

## Task 4: Visibility demonstration

**File:** `Assignment_13_Advanced CSS/Task_4.html`

The current page contains an explanation and a reference image. The stated concept is the `visibility: hidden` property.

### Concepts to compare

| Property | Visible? | Layout space retained? |
|---|---:|---:|
| `visibility: hidden` | No | Yes |
| `display: none` | No | No |
| `opacity: 0` | Transparent | Yes |

Opacity alone does not remove an element from keyboard focus or pointer interaction. Do not use it as an accessible hiding technique without addressing interaction.

## Task 5: Visual output exercise

**File:** `Assignment_13_Advanced CSS/Task_5.html`

This page contains a short description and a corresponding image from the `Output` folder. Use both files to inspect the exercise. The source currently does not provide enough context to assert a more specific CSS learning objective.

## Working with output images

Each task's captured output uses a matching filename:
- `Output/task_1.png`
- `Output/task_2.png`
- `Output/task_3.png`
- `Output/task_4.png`
- `Output/task_5.png`

Update a reference screenshot only when you intentionally change the expected result. Keep filenames and case consistent because case-sensitive hosting environments distinguish different filename capitalization.

## Suggested experiments

- Add responsive constraints to fixed-size examples.
- Add semantic labels and meaningful alternative text.
- Respect reduced-motion preferences.
- Add visible keyboard focus if interactive controls are introduced.
- Document browser-specific differences rather than assuming all engines render identically.
