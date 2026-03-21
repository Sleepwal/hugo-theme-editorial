# Hugo Theme Editorial

A sophisticated, magazine-style Hugo theme with bold typography and clean editorial design.

## Features

- **Editorial/Magazine Style** - Bold typography, clean layouts, sophisticated design
- **Responsive Design** - Mobile-first approach with seamless desktop experience
- **Dark Mode Support** - Toggle between light and dark themes
- **Table of Contents** - Fixed sidebar TOC for easy navigation
- **Categories & Tags** - Organized taxonomy with elegant presentation
- **Search** - Built-in search functionality
- **Internationalization** - Support for multiple languages

## Installation

### As a Git Submodule

```bash
git submodule add https://github.com/Sleepwal/hugo-theme-editorial.git themes/hugo-theme-editorial
```

### As a Clone

```bash
git clone https://github.com/Sleepwal/hugo-theme-editorial.git themes/hugo-theme-editorial
```

## Configuration

Add the theme to your `hugo.toml`:

```toml
theme = "hugo-theme-editorial"
```

### Example Configuration

```toml
baseURL = 'https://example.com/'
title = 'My Editorial Blog'
theme = "hugo-theme-editorial"
languageCode = 'zh-CN'

[params]
  author = "Your Name"
  description = "Your blog description"
  mainSections = ["post"]

[menu]
[[menu.main]]
  identifier = "home"
  name = "首页"
  url = "/"
  weight = 1
[[menu.main]]
  identifier = "archives"
  name = "归档"
  url = "/archives/"
  weight = 2
[[menu.main]]
  identifier = "tags"
  name = "标签"
  url = "/tags/"
  weight = 3
[[menu.main]]
  identifier = "categories"
  name = "分类"
  url = "/categories/"
  weight = 4
```

## Customization

### Fonts

The theme uses Google Fonts by default:
- **Display**: Playfair Display
- **Body**: DM Sans
- **Code**: JetBrains Mono (if needed)

### Colors

Main accent color is a classic editorial red (`#c41e3a`).

### Layout

- Top navigation bar with brand and menu
- Left sidebar with author info, search, categories, and tags
- Main content area with article list or article content
- Right sidebar for table of contents (on article pages)

## Development

### Prerequisites

- Hugo 0.110.0 or higher
- Dart Sass (for SCSS compilation)

### Build

```bash
hugo server
```

## License

GNU General Public License v3 - see [LICENSE](LICENSE) for details.
