# Portfolio (v1)

My first personal portfolio site, built with plain HTML and CSS as a course project in May 2026.
It's here as a record of where I started; a new, project-focused portfolio will replace it.

## Pages

| Page | What's on it |
| --- | --- |
| `index.html` | Home: introduction and photo |
| `about.html` | About me |
| `skills.html` | Skills |
| `projects.html` | Project cards |
| `resume.html` | Resume |
| `contact.html` | Contact form (layout only, it doesn't send anything) and links |

Each page has its own stylesheet in `css/`. Images are in `images/`.

## Run it

No build step. Open `index.html` in a browser, or serve the folder:

```bash
python -m http.server 8000
```

Then go to http://localhost:8000.

## Known limitations

- Most "View Project" buttons don't link anywhere yet, and one links to a placeholder.
- The contact form has no backend.
- One stylesheet per page means shared styles (header, footer) are repeated.

## What I learned

Semantic page structure, Flexbox layouts, linking pages together, and why valid HTML matters:
an HTML validator caught unclosed tags and a `<body>` that closed before the footer.

## Checks

Every push runs [html-validate](https://html-validate.org/) (`.github/workflows/html-check.yml`).
Run it locally with `npx html-validate@11 "**/*.html"`.
