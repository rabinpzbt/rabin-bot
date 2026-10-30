# Display Article Description in Post View (Minimal Scope)

Render the article `description` frontmatter field in the post layout directly beneath the title and above the metadata, styled as a subtle italicized lead subtitle, with zero edits to any other files or content.

## User Review & Critical Decisions

> [!IMPORTANT]
> Scope has been strictly pruned to only the essential template and style updates requested:
> - **Only 2 Files Touched**:
>   1. `_includes/layouts/post.njk` — Add the conditional description element.
>   2. `public/css/index.css` — Add the minimal subtitle style definition.
> - **Zero Content Modifications**: Existing markdown articles (`content/blog/*.md`) and other files will NOT be edited or altered.

- **Placement**: Directly below `<h1 class="postTitle">` and before `<ul class="post-metadata">`.
- **Styling**: `.post-description` with italic posture, comfortable margin, and the existing theme-aware variable `var(--color-gray-90)`.

---

## 1. Overview & Core Concept

- **What It Does**: Renders the article `description` frontmatter in the post view whenever present.
- **Scope Limit**: Solely updates the post template and its corresponding stylesheet class.

---

## 2. User Experience & Visual Design

- **Layout**:
  - Title (`.postTitle`)
  - Description (`.post-description`): Italic, muted color (`var(--color-gray-90)`), 1.25em size, clean spacing.
  - Metadata (`.post-metadata`): Publication date and tags.
- **Light & Dark Theme**: Automatically inherits the theme color scheme via CSS variable without extra classes.

---

## 3. Minimal Change Specification

1. **`_includes/layouts/post.njk`**:
   ```html
   {% if description %}
   <p class="post-description">{{ description }}</p>
   {% endif %}
   ```
2. **`public/css/index.css`**:
   ```css
   .post-description {
       font-style: italic;
       color: var(--color-gray-90);
       margin: 0.5em 0 1em;
   }
   ```
