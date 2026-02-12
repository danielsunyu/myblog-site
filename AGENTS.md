# AGENTS.md - Myblog-site

## Build & Serve Commands

- `hugo` - Build static site to `/public` directory
- `hugo server` - Local dev server (http://localhost:1313)
- `hugo server -D` - Dev server including draft posts

## Architecture & Structure

- **Hugo Static Site Generator** - Framework for the blog
- **Theme**: Maverick (`/themes/maverick`) - Submodule with layouts and assets
- **Content**: `/content` - Blog posts and pages in Markdown format
- **Layouts**: `/layouts` - Template overrides (uses Maverick theme as fallback)
- **Static Assets**: `/static` - Images, favicon, other static files
- **Configuration**: `hugo.toml` - TOML configuration (baseURL, theme, menu, markup settings)
- **No database** - Static site; uses Disqus for comments

## Code Style & Conventions

- **Markdown**: Use standard Hugo Markdown syntax; enable mathjax with `math = true` in frontmatter
- **TOML**: Configure site via `hugo.toml` following Hugo conventions
- **Frontmatter**: YAML or TOML at top of content files; use `draft`, `tags`, `categories` fields
- **Naming**: Content files snake_case (e.g., `my-post.md`); category/tag slugs lowercase
- **Git**: Theme is a git submodule; don't edit theme files directly
