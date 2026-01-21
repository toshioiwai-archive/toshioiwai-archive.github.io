---
title: "Design Documentation"
---

## Typography

### Font
- **Family**: Inter (Google Fonts)
- **Weight**: 400 only (uniform weight)
- **Letter-spacing**: 0 (no tracking)

### Scale
| Class | Size | Usage |
|-------|------|-------|
| `text-xl` | 1.25rem (20px) | Header site title, page titles |
| `text-lg` | 1.125rem (18px) | Card titles in lists |
| `text-base` | 1rem (18px) | Body text, English subtitles |
| `text-sm` | 0.875rem | Meta info, badges, breadcrumbs |

Base font size is set to 18px via `html { font-size: 18px }`.

---

## Colors

Using daisyUI `lofi` theme.

| Token | Usage |
|-------|-------|
| `bg-base-100` | White background (main) |
| `bg-base-200` | Light gray (hover states) |
| `text-base-content` | Black text |
| `text-base-content/70` | Gray text (English titles) |
| `text-base-content/60` | Light gray text (meta info) |
| `border-base-300` | Border color |

---

## Cards

Used for list items (Works, Exhibitions, Media).

```html
<a href="..." class="card card-compact bg-base-100 hover:bg-base-200 transition-colors border border-base-300 block">
    <div class="card-body">
        <h2 class="card-title text-lg">Title</h2>
        <p class="text-base-content/70 text-sm">English Title</p>
        <!-- badges, meta info -->
    </div>
</a>
```

### Behavior
- Entire card is clickable (`<a>` wrapper)
- Hover: background changes to `bg-base-200`
- Transition: `transition-colors`

### Grid Layout
| Page | Columns |
|------|---------|
| Works | 3 cols on lg, 2 on md, 1 on mobile |
| Exhibitions | 2 cols on md, 1 on mobile |
| Media | 3 cols on lg, 2 on md, 1 on mobile |

---

## Badges

```html
<div class="badge badge-outline">Year</div>
<div class="badge badge-ghost">Type</div>
<div class="badge badge-outline badge-sm">Small Badge</div>
```

---

## Detail Page Layout

Single column layout:

1. **Breadcrumb** - `text-sm mb-6`
2. **Title** - `text-xl mb-2`
3. **English Title** - `text-base text-base-content/70 mb-8`
4. **Description** - `mb-8`
5. **Data List** - Definition list with dividers

### Data List

```html
<dl class="divide-y divide-base-300">
    <div class="py-3 flex">
        <dt class="w-32 text-base-content/60">Label</dt>
        <dd>Value</dd>
    </div>
</dl>
```

---

## Header

- Site title: `text-xl hover:underline`
- Navigation: `hover:underline`
- On home page: site title is `<h1>`
- On other pages: site title is `<p>`

---

## Footer

- Centered
- Copyright text
- `bg-base-100` (white background)

---

## Breadcrumbs

Using daisyUI breadcrumbs component.

```html
<div class="breadcrumbs text-sm mb-6">
    <ul>
        <li><a href="/">Home</a></li>
        <li><a href="/works/">Works</a></li>
        <li>Current Page</li>
    </ul>
</div>
```

---

## Container

- Max width: `max-w-[1440px]`
- Padding: `px-6 md:px-12`
- Centered: `mx-auto`

---

## Links

- Default: no underline
- Hover: `hover:underline`
- Use `.RelPermalink` for internal links (relative paths)
