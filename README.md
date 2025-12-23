# Toshio Iwai Archive

Archive website for Toshio Iwai's works.

This site publishes information about artworks, exhibitions, and media coverage.

## Repository Structure

```
├── opendata/          # Open data (CSV)
│   └── LICENSE.md     # CC BY 4.0
├── website/           # Hugo static site
│   ├── content/       # Site content
│   ├── themes/        # Hugo themes
│   └── hugo.toml      # Hugo configuration
└── LICENSE.md         # Apache 2.0 (for code)
```

## Website Development

See `website/readme.md` for details.

### Local Development

```bash
cd website
hugo server -D
```

Open http://localhost:1313/ in your browser to preview.

### Production Build

```bash
cd website
hugo
```

Build output is generated in `website/public/`.

## Deployment

Automatically built and deployed via GitHub Actions.

- **Public URL**: https://toshioiwai-archive.github.io/

## Tech Stack

- **Static Site Generator**: Hugo v0.145.0+
- **Hosting**: GitHub Pages
- **CI/CD**: GitHub Actions

## License

This repository uses two different licenses:

| Content | License |
|---------|---------|
| Code & configuration files | [Apache License 2.0](LICENSE.md) |
| Open data (`opendata/`) | [CC BY 4.0](opendata/LICENSE.md) |

## Open Data

The `opendata/` directory contains metadata for artworks, exhibitions, and media coverage in CSV format.

- **Direct from GitHub**: `opendata/*.csv`
- **Via website**: https://toshioiwai-archive.github.io/opendata/
