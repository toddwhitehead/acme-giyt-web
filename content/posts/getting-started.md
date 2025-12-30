---
title: "Getting Started with Hugo"
date: 2024-01-20T10:00:00-00:00
draft: false
---

Hugo makes it incredibly easy to build and maintain static websites. Here's a quick guide to get you started.

## Installation

Hugo is available for macOS, Windows, and Linux. You can install it using various package managers or download it directly from the official website.

## Creating Your First Site

Creating a new Hugo site is as simple as running:

```bash
hugo new site mysite
```

## Adding Content

You can create new content using the `hugo new` command:

```bash
hugo new posts/my-first-post.md
```

## Building and Serving

To preview your site locally:

```bash
hugo server -D
```

To build your site for production:

```bash
hugo
```

The built site will be in the `public` directory, ready to be deployed!
