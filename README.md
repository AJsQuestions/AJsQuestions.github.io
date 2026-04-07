# AJ's Questions — Personal Website

Source for [ajsquestions.github.io](https://ajsquestions.github.io), built with [Hugo](https://gohugo.io/) and a modified [PaperMod](https://github.com/adityatelange/hugo-PaperMod/) theme.

## Local Development

### Prerequisites

- [Hugo Extended](https://gohugo.io/installation/) (v0.139.0+)
- [Dart Sass](https://sass-lang.com/dart-sass/) (for stylesheet compilation)
- Git (with submodule support for the theme)

### Setup

```bash
# Clone with submodules (theme)
git clone --recurse-submodules https://github.com/AJsQuestions/AJsQuestions.github.io.git
cd AJsQuestions.github.io

# Start the dev server
hugo server -D
```

The site will be available at `http://localhost:1313/`. The `-D` flag includes draft posts.

### Creating Content

```bash
# New blog post
hugo new blog/my-post-title.md

# New research paper (uses paper archetype)
hugo new research/paper-name.md
```

### Build for Production

```bash
hugo --gc --minify
```

Output goes to `public/`.

## Project Structure

```
.
├── archetypes/        # Templates for new content (blog, paper, course)
├── assets/css/        # Theme CSS (variables, common styles, media queries)
├── content/           # Markdown content
│   ├── about/         # About page
│   ├── blog/          # Blog posts
│   ├── contact/       # Contact page
│   ├── projects/      # Projects showcase
│   ├── questions/     # Question constellations
│   ├── research/      # Research papers
│   └── teaching/      # Teaching materials
├── layouts/           # Hugo templates (overrides theme defaults)
│   ├── partials/      # Reusable template fragments
│   └── shortcodes/    # Custom shortcodes (constellation, rawhtml)
├── static/            # Static assets (images, CV PDF, favicons)
└── config.yml         # Site configuration
```

## Deployment

Deployed automatically via GitHub Actions on push to `main`. The workflow runs `hugo --gc --minify` and publishes to GitHub Pages.

## License

[MIT](LICENSE.md)
