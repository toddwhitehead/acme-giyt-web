# Post Images

This directory contains images used in blog posts.

## Usage

When creating a blog post, you can reference images from this directory using:

```markdown
![Alt text](/images/posts/your-image.jpg)
```

## Organization

- Store images with descriptive filenames
- Consider organizing by post date or topic if needed (e.g., `2024-01-15-post-name/`)
- Supported formats: JPG, PNG, GIF, SVG, WebP

## Best Practices

- **Optimize images** before uploading to reduce file size and improve page load times
- Use descriptive filenames (e.g., `hugo-logo.png` instead of `img001.png`)
- Consider using lowercase and hyphens for filenames (e.g., `my-screenshot.jpg`)
- Keep images under 1MB when possible
- Use appropriate formats:
  - JPG for photographs
  - PNG for graphics with transparency
  - SVG for logos and icons
  - WebP for modern browsers with better compression

## Example Structure

```
posts/
├── 2024-01-15-getting-started/
│   ├── hero-image.jpg
│   └── screenshot.png
├── 2024-02-20-tutorial/
│   ├── step1.png
│   └── step2.png
└── logo.svg
```
