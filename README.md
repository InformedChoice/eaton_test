# Rogers Daily Reading

A bilingual reading website for Solomon, Christian, Miriam, and Shiloh, built with Hugo. This site provides reading content in both English and Spanish to support bilingual literacy development.

## Site Structure

The website is organized as follows:

- `content/en/post/` - Contains The Old Man and the Sea parts (current book)
- `content/en/books/` - Directory for book entries and information
- `archetypes/` - Templates for creating new content
- `layouts/` - Custom HTML templates for rendering the site
- `static/` - Images and other static assets

## Getting Started

1. Install Hugo: https://gohugo.io/installation/
2. Clone this repository
3. Run `hugo server -D` to start the development server
   - This will make the site available at http://localhost:1313/

## Adding New Content

### Adding a Part to "The Old Man and the Sea"

To add a new part to the current book:

```bash
hugo new --kind book-section post/part-XX-title.md
```

Replace:
- `XX` with the part number (e.g., 14, 15, etc.)
- `title` with a short title for the section (e.g., `shark-attack`, `return-home`)

Example:
```bash
hugo new --kind book-section post/part-14-final-return.md
```

This will create a new file with proper front matter and the bilingual format template.

### Creating a New Book

To start a new book:

```bash
hugo new --kind new-book books/book-title.md
```

Replace `book-title` with a hyphenated name for the book (e.g., `the-little-prince`, `don-quixote`).

Example:
```bash
hugo new --kind new-book books/pride-and-prejudice.md
```

Then edit the generated file with:
- Author information
- Book description
- Any other relevant details

### Adding Parts to a New Book

After creating a new book, you can add parts to it:

1. Create a new directory for the book:
```bash
mkdir -p content/en/books/book-title
```

2. Add new parts to the book:
```bash
hugo new --kind book-section books/book-title/part-1-introduction.md
```

## Content Format

Each section follows a bilingual format with:
- English and Spanish side by side for each line
- Numbered lines for easy reference
- Table of contents for navigation
- Back links to return to the table of contents

## Managing Images

1. Place book cover images in the `static/images/` directory
2. Reference them in content using: `/images/filename.jpg`

## Building for Production

To build the site for deployment:

```bash
hugo --minify
```

The output will be in the `public` directory, which can be deployed to any static hosting service (Netlify, GitHub Pages, etc.).

## Maintenance

- Keep book parts consistently numbered (Part 7, Part 8, etc.)
- Maintain the same bilingual format across all content
- Use descriptive filenames that match content
- Add images to the `static/images/` directory as needed
