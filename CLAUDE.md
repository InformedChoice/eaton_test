# CLAUDE.md - Hugo Static Site Development Guide

## Build Commands

- Build site: `hugo`
- Run dev server: `hugo server -D` (includes draft content)
- Build for production: `hugo --minify`
- Create new content: `hugo new content/en/post/new-post.md`

## Site Structure

- Content is organized by language (`/content/en/`, `/content/fr/`)
- Templates are in `/layouts/` (override theme templates here)
- Static assets go in `/static/`
- The site uses the Ananke theme

## Style Guidelines

- Front matter should use TOML format with consistent indentation
- Content should be written in Markdown with proper heading hierarchy
- Use relative URLs for internal links: `[Link](/post/page/)`
- Image paths should be relative to static directory: `/images/filename.jpg`
- Keep file names lowercase with hyphens: `my-new-post.md`

## Shortcodes

- Use built-in Hugo shortcodes for consistent rendering
- Custom shortcodes available in `/layouts/shortcodes/`
- Example: `{{< form-contact >}}`

## Site Goals

### Instructions for LLM: Transforming the Eaton Fires Hugo Site into Rogers Daily Reading

#### Site Overview

The current Hugo website hosted on Netlify was originally designed for Eaton Fires testing purposes. It now needs to be fully converted to a new site called **Rogers Daily Reading**, dedicated to providing bilingual reading content (English and Spanish) for elementary school-aged children: Solomon, Christian, Miriam, and Shiloh.

#### Site Purpose

The site’s primary function is to offer daily reading material from classic literature that is in the public domain. Each page of content will display the original English text alongside its Spanish translation. The children are required to read both versions nightly.

#### Current Book

Start with **The Old Man and the Sea** by Ernest Hemingway. Ensure this book is prominently displayed and easily accessible.

#### Required Changes & Features

1. **Complete Conversion:**

   - Remove all Eaton Fires-related content, branding, or references.
   - Rebrand and redesign the site to clearly reflect the new name **Rogers Daily Reading**.

2. **Book Organization:**

   - Homepage should prominently feature the current book selection with a clear, clickable link to begin reading.
   - Structure the site to easily add future books in the same format.
   - Maintain a simple archive or catalog page listing all available books.

3. **Reading Experience:**

   - Provide infinite scrolling or easy pagination through chapters or sections of the book.
   - Clearly present English and Spanish texts side-by-side or toggleable for readability.
   - Implement a bookmarking or progress-saving feature enabling readers to easily return to their last-read position.

4. **Navigation & User Experience:**

   - Navigation should be intuitive, visually appealing, and child-friendly.
   - Utilize large, readable fonts, gentle colors, and an uncluttered layout suitable for elementary students.
   - Provide clear instructions on how to navigate the content (next chapter, previous chapter, home page).

5. **Visual Appeal:**

   - Design should be engaging and visually appealing to children aged 7–10.
   - Incorporate illustrations or themed graphics related to the book's content (e.g., ocean-themed visuals for "The Old Man and the Sea").

6. **Accessibility and Responsiveness:**
   - Ensure the website is fully responsive and functions smoothly on tablets and mobile devices, as well as desktop computers.

#### Long-Term Scalability

- Set up the structure clearly so additional books can be seamlessly added later without extensive site redesign.

#### Children Using the Site

- Solomon
- Christian
- Miriam
- Shiloh
