# Toshio Iwai Archive - Open Data

This directory contains archive data for Toshio Iwai in CSV and JSON formats.

## Files

| File | Format | Contents |
|------|--------|----------|
| `works.csv` / `works.json` | CSV / JSON | Artworks data |
| `events.csv` / `events.json` | CSV / JSON | Exhibitions data |
| `media.csv` / `media.json` | CSV / JSON | Media coverage data |

## Data Formats

- **CSV**: UTF-8 encoded, suitable for spreadsheets and data analysis
- **JSON**: UTF-8 encoded, suitable for web applications and APIs

### works

| Field | Description |
|-------|-------------|
| id | Work ID |
| title | Title (Japanese) |
| title_en | Title (English) |
| year | Year created |
| type | Work type |
| description | Description |

### events

| Field | Description |
|-------|-------------|
| id | Exhibition ID |
| title | Title (Japanese) |
| title_en | Title (English) |
| venue | Venue name (Japanese) |
| venue_en | Venue name (English) |
| start_date | Start date |
| end_date | End date |
| location | Location (Japanese) |
| location_en | Location (English) |
| description | Description |

### media

| Field | Description |
|-------|-------------|
| id | Media ID |
| type | Type (article, book, video, etc.) |
| title | Title (Japanese) |
| title_en | Title (English) |
| publication | Publication name (Japanese) |
| publication_en | Publication name (English) |
| date | Publication date |
| url | URL (if available) |

## License

[CC BY 4.0](LICENSE.md) - Free to use with attribution.
