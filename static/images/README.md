# Background Images

This directory contains background images for the website's dark and light modes.

## Current Setup

The website is currently configured to use CSS gradients for the background:
- **Light mode**: Blue to purple gradient
- **Dark mode**: Dark blue to gray gradient

## Using Custom Images

To use custom background images instead of gradients:

1. Place your images in this directory:
   - `bg-light.jpg` - Background for light mode
   - `bg-dark.jpg` - Background for dark mode

2. Update `assets/css/extended/custom.css` and replace the gradient definitions:

```css
/* Light mode background */
[data-theme="light"] .main {
    background-image: url('/images/bg-light.jpg');
}

/* Dark mode background */
[data-theme="dark"] .main {
    background-image: url('/images/bg-dark.jpg');
}

/* Auto mode - default to light */
[data-theme="auto"] .main {
    background-image: url('/images/bg-light.jpg');
}

/* Media query for auto mode to respect system preference */
@media (prefers-color-scheme: dark) {
    [data-theme="auto"] .main {
        background-image: url('/images/bg-dark.jpg');
    }
}
```

## Image Recommendations

- **Format**: JPG or PNG
- **Size**: 1920x1080 or higher for best quality
- **Optimization**: Compress images to reduce loading time
- **Content**: Choose images that don't interfere with text readability
- **Themes**: Light mode images should be bright/light, dark mode images should be subtle/dark

## Testing

After adding images:
1. Run `hugo server` to test locally
2. Toggle between light and dark modes to see both backgrounds
3. Check text readability on both backgrounds
4. Adjust the overlay opacity in CSS if needed for better contrast 