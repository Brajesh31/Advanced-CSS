# Troubleshooting

## Page does not open

Confirm the filename and quote the path because the directory name contains a space. A local server avoids file-path and relative-asset issues.

## Styles look different

Check browser zoom, viewport size, default browser styles, and whether the expected stylesheet or embedded CSS loaded. Compare against the matching output image.

## Images are missing

Use the exact relative path and preserve the `Output` directory name and filename casing.

## Layout overflows on small screens

Test the narrow viewport, inspect fixed widths and absolute positioning, and add responsive rules without changing the exercise's intended demonstration.
