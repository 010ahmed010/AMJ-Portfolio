# Ahmed Al-Jassem Portfolio

## Project Overview
A personal portfolio website for Ahmed Al-Jassem, a Full-Stack Web Developer. Features a modern terminal / glassmorphism aesthetic.

## Tech Stack
- **Frontend**: Plain HTML5, CSS3, JavaScript (ES6+)
- **Styling**: Tailwind CSS (via CDN), custom CSS
- **Icons**: Lucide Icons, Font Awesome (via CDN)
- **Fonts**: Google Fonts (Inter, Fira Code)
- **Data**: Projects fetched dynamically from external JSON API at `https://010ahmed010.github.io/api/AMJ-Portfolio.json`
- **No build system or package manager** — all dependencies loaded via CDN

## Project Structure
```
index.html        # Main portfolio (single-page: Hero, About, Skills, Projects, Services, Contact)
resume.html       # Full CV / Resume page — web view (dark) + clean PDF print layout (white)
project.html      # Dynamic project detail page (reads ?title= from URL, fetches from API)
uses.html         # Tools & Setup page (editor, frameworks, hardware, hosting)
assets/logos/     # Tech brand icons (MongoDB, Node.js, React, Tailwind)
attached_assets/  # UI screenshots / design references
```
Note: `Portfolio.html` was removed — `index.html` is the canonical main page (required for GitHub Pages).

## Running Locally
Served via Python's built-in HTTP server on port 5000:
```
python3 -m http.server 5000 --bind 0.0.0.0
```

## Deployment
Configured as a **static** deployment with `publicDir: "."`.
The `Portfolio.html` file is served as the root of the static site.

## Key Features
- Terminal simulation (hero section auto-types developer info)
- Dynamic project gallery filtered from external JSON API
- Scroll-based animations and Intersection Observer section reveals
- Glassmorphism UI aesthetic
