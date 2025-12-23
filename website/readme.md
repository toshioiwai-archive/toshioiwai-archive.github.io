# Toshio Iwai Archive Website

Archive website for Toshio Iwai.

## Tech Stack
- Framework: Hugo (v0.145.0+)
- Deployment: GitHub Actions
- Hosting: GitHub Pages
- Theme: toshioiwai (custom theme)
- Languages: Japanese (default) + English

## Directory Structure

```
website/
├── archetypes/      # Content templates
├── assets/          # CSS, JS and other processed assets
├── content/         # Site content (Markdown)
├── data/            # Data files (CSV, JSON, etc.)
├── i18n/            # Internationalization translation files
├── layouts/         # HTML templates
├── static/          # Static files (images, fonts, etc.)
├── themes/          # Theme directory
│   └── toshioiwai/  # Custom theme
└── hugo.toml        # Hugo configuration file
```

## Development Commands

### Start Development Server

```bash
cd website
hugo server -D
```

Development server is accessible at http://localhost:1313/

### Production Build

```bash
cd website
hugo
```

Built files are output to the `public/` directory.

### Build Including Drafts

```bash
cd website
hugo -D
```

## Content Management

Content is stored in Markdown format under the `content/` directory in the following sections:

- `content/works/` - Artworks information
- `content/events/` - Exhibitions information
- `content/media/` - Media coverage information

Each content item has both Japanese (.ja.md) and English (.en.md) files.

## Deployment

Automatically deployed via GitHub Actions.
Build and deployment are triggered automatically when pushing to the `main` branch.
