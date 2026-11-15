# ♿ Accessibility Guidelines

These guidelines help keep small CSS exercises understandable and usable by a wide range of people. Accessibility is not limited to large applications. A simple HTML page can still create barriers through low contrast, motion, missing image text, or poor keyboard interaction.

## 📚 Contents

- [Semantic HTML](#semantic-html)
- [Keyboard access](#keyboard-access)
- [Colour and contrast](#colour-and-contrast)
- [Motion](#motion)
- [Images](#images)
- [Visibility techniques](#visibility-techniques)
- [Review checklist](#review-checklist)

## Semantic HTML

Use elements according to their meaning. Buttons should perform actions, links should navigate, headings should describe sections, and lists should represent collections. Avoid using generic containers where a semantic element communicates the purpose more clearly.

## Keyboard access

If a task introduces interactive controls:
- Ensure the controls are reachable by keyboard.
- Preserve a visible focus indicator.
- Use native controls when practical.
- Do not require mouse hover to reveal essential information.
- Keep focus order logical.

## Colour and contrast

Text and controls should remain distinguishable from their background. Do not use colour as the only way to communicate status or meaning. Test both normal and high-contrast settings where possible.

## Motion

The cube and loader exercises use continuous animation. Respect the user's motion preference:

```css
@media (prefers-reduced-motion: reduce) {
  .loader,
  .cube {
    animation: none;
  }
}
```

When animation is disabled, preserve a clear static representation of the content.

## Images

Meaningful images need useful alternative text. Decorative images should use an empty alternative text value. Avoid generic alt text such as "image" when the image communicates a specific result.

## Visibility techniques

The CSS visibility properties have different accessibility and layout behaviour. Hiding something visually does not always remove it from the keyboard tab order or accessibility tree. Choose an approach that matches the desired interaction and semantics.

## Review checklist

- [ ] Headings are in a logical order.
- [ ] Interactive elements are keyboard reachable.
- [ ] Focus remains visible.
- [ ] Colour contrast is readable.
- [ ] Images have suitable alternative text.
- [ ] Motion is reduced when requested.
- [ ] Hidden content does not create confusing keyboard stops.
- [ ] Content remains usable when zoomed.
