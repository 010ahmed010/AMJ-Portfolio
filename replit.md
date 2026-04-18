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
Portfolio.html        # Main entry point (all HTML, CSS, JS in one file)
assets/logos/         # Tech brand icons (MongoDB, Node.js, React, Tailwind)
attached_assets/      # UI screenshots / design references
```

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
