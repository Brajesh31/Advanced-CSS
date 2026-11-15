# 🎨 CSS Technique Reference

This document is a concise reference for the CSS techniques currently used by the assignments and safe experiments for learning more about them.

## 📚 Contents

- [Custom properties](#custom-properties)
- [The var function](#the-var-function)
- [Three-dimensional transforms](#three-dimensional-transforms)
- [Perspective](#perspective)
- [Keyframe animations](#keyframe-animations)
- [Circular shapes](#circular-shapes)
- [Visibility and layout](#visibility-and-layout)
- [Reduced motion](#reduced-motion)
- [Browser inspection](#browser-inspection)

## Custom properties

Custom properties store reusable CSS values.

```css
:root {
  --primary-color: #00b7ff;
  --secondary-color: #6c757d;
}

.primary-button {
  background-color: var(--primary-color);
}
```

The `:root` selector makes the values available through inheritance to descendants. A custom property can also be scoped to a component or container when global access is not needed.

## The var function

The `var()` function reads a custom property and can provide a fallback.

```css
.card {
  color: var(--text-color, #222);
}
```

The fallback is used when the referenced custom property is missing or invalid at computed-value time. It is not a general CSS parser error recovery mechanism.

## Three-dimensional transforms

CSS transforms can rotate and translate elements in three dimensions.

```css
.cube-scene {
  perspective: 900px;
}

.cube {
  transform-style: preserve-3d;
  transform: rotateX(20deg) rotateY(30deg);
}

.front {
  transform: translateZ(100px);
}
```

When building a cube, face dimensions and translation distances must correspond. Transform order affects the final position and orientation.

## Perspective

The `perspective` property establishes the distance between the viewer and the z=0 plane for transformed descendants. A smaller positive distance generally produces a more pronounced perspective effect. A larger distance produces a subtler effect.

Perspective should be tested at the actual element size. Values that look effective on a large monitor can produce exaggerated distortion on a small viewport.

## Keyframe animations

A keyframe animation describes how a property changes over time.

```css
@keyframes spin {
  from { transform: rotate(0deg); }
  to { transform: rotate(360deg); }
}

.loader {
  animation: spin 1.2s linear infinite;
}
```

Use animation only when it communicates state or improves the experience. Continuous motion should respect user motion preferences.

## Circular shapes

A box can be made circular when it has equal width and height and uses `border-radius: 50%`.

```css
.loader {
  width: 48px;
  aspect-ratio: 1;
  border: 6px solid #e5e7eb;
  border-top-color: #2563eb;
  border-radius: 50%;
}
```

## Visibility and layout

`visibility: hidden` preserves layout space. `display: none` removes the element from layout. `opacity: 0` only changes transparency and can leave an element interactive.

Choose a hiding strategy based on both visual and accessibility requirements.

## Reduced motion

For non-essential animations, provide a reduced-motion alternative:

```css
@media (prefers-reduced-motion: reduce) {
  .loader,
  .cube {
    animation: none;
  }
}
```

A real application may need a static visual state or accessible status text when motion is disabled.

## Browser inspection

Use browser developer tools to:
- Inspect computed styles.
- Identify overridden declarations.
- Check element dimensions and overflow.
- Pause and inspect animations.
- Test responsive viewport sizes.
- Review console warnings and errors.
- Emulate reduced-motion preferences.
