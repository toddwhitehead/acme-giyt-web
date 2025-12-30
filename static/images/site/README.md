# Site Images

This directory contains general website images used across the site.

## Usage

Reference images from this directory in your templates or content using:

```markdown
![Alt text](/images/site/your-image.jpg)
```

Or in HTML templates:

```html
<img src="/images/site/your-image.jpg" alt="Description">
```

## Organization

This directory is for images that are used site-wide, such as:

- **Logo files** - Site logo, favicon sources
- **Backgrounds** - Hero images, section backgrounds
- **Icons** - Navigation icons, social media icons
- **UI Elements** - Buttons, decorative elements
- **Default images** - Placeholder or fallback images

## Best Practices

- **Optimize images** before uploading to reduce file size
- Use descriptive filenames that indicate purpose (e.g., `site-logo.svg`, `hero-background.jpg`)
- Keep multiple sizes/versions for responsive design (e.g., `logo-sm.png`, `logo-lg.png`)
- Use consistent naming conventions
- Maintain organized subdirectories if needed:
  - `logos/` - Brand logos and variations
  - `backgrounds/` - Background images
  - `icons/` - Icon sets
  - `ui/` - User interface elements

## Example Structure

```
site/
├── logos/
│   ├── site-logo.svg
│   ├── site-logo-dark.svg
│   └── favicon.png
├── backgrounds/
│   ├── hero-home.jpg
│   └── section-bg.jpg
└── icons/
    ├── github.svg
    ├── twitter.svg
    └── linkedin.svg
```
