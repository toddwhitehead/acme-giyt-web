# acme-giyt-web

A static website built with [Hugo](https://gohugo.io/), a fast and flexible static site generator.

## Prerequisites

- [Hugo](https://gohugo.io/installation/) (Extended version recommended)

## Getting Started

### Installation

Install Hugo by following the [official installation guide](https://gohugo.io/installation/) for your operating system.

### Running Locally

To preview the site locally with live reload:

```bash
hugo server -D
```

The site will be available at `http://localhost:1313/`

### Building for Production

To build the static site for production:

```bash
hugo
```

The generated static files will be in the `public/` directory, ready for deployment.

### Creating New Content

To create a new blog post:

```bash
hugo new posts/my-new-post.md
```

To create a new page:

```bash
hugo new about.md
```

## Project Structure

```
.
├── archetypes/      # Content templates
├── assets/          # Assets to be processed (SCSS, JS, etc.)
├── content/         # Markdown content files
├── data/            # Data files (JSON, YAML, TOML)
├── layouts/         # HTML templates
├── static/          # Static files (images, CSS, JS)
├── themes/          # Hugo themes
└── hugo.toml        # Site configuration
```

## Deployment

This static site can be deployed to any web hosting service that supports static files:

- **GitHub Pages**: Commit the `public/` folder or use GitHub Actions
- **Netlify**: Connect your repository and Netlify will build automatically
- **Vercel**: Import your repository for automatic deployments
- **AWS S3**: Upload the `public/` folder to an S3 bucket
- **Any static host**: Upload the contents of `public/` directory

## License

See [LICENSE](LICENSE) file for details.
