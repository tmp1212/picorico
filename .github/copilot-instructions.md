# Copilot Instructions for PICORICO Repository

## Overview
This repository contains the official website for PICORICO, a premium coffee and dessert brand. The site is a single-page application (SPA) supporting three languages: Korean, English, and Thai. It showcases the brand's story, menu, catering services, team, global vision, and store locations.

## Key Files and Structure
- **`index.html`**: The main HTML file containing all sections of the website.
- **`css/style.css`**: Contains all the styling rules for the website.
- **`js/main.js`**: Handles interactivity, animations, and language switching.
- **`images/`**: Stores all image assets used across the website.
- **`README.md`**: Provides an overview of the project, including recent updates and future development recommendations.

## Development Patterns
### Language Switching
- Language support is implemented using the `data-lang` attribute and the `setLang()` function in `main.js`.
- The `<body>` tag uses a class (`lang-ko`, `lang-en`, `lang-th`) to determine the active language.

### Section Anchors
- Each section of the page is identified by an `id` attribute (e.g., `#hero`, `#brand-story`).
- Navigation relies on these anchors for smooth scrolling.

### Image Updates
- Images are stored in the `images/` directory. Recent updates include:
  - `images/expert_team.jpg`: Background for the expert team card.
  - `images/miumiu.jpg`: Used in the luxury catering section.
  - `images/eunpyeong_1.jpg`: New store image for the Eunpyeong location.

## Critical Workflows
### Testing Changes
1. Open `index.html` in a browser to preview changes.
2. Use browser developer tools to inspect and debug styles and scripts.

### Adding New Sections
1. Add a new `<section>` block in `index.html` with a unique `id`.
2. Update `css/style.css` to style the new section.
3. If interactivity is required, add corresponding JavaScript in `js/main.js`.

### Updating Images
1. Place the new image in the `images/` directory.
2. Update the `src` attribute in `index.html` to reference the new image.

## Project-Specific Conventions
- **CSS Naming**: Use BEM (Block Element Modifier) methodology for class names.
- **JavaScript**: Keep functions modular and reusable. Avoid inline JavaScript in `index.html`.
- **HTML**: Maintain semantic structure with appropriate tags (e.g., `<header>`, `<section>`, `<footer>`).

## External Dependencies
- **Google Fonts**: Cormorant Garamond, Inter, DM Mono.
- **Font Awesome 6**: Used for icons.
- **Pexels CDN**: Hosts some external images.

## Future Enhancements
Refer to the `향후 개발 권장 사항` section in `README.md` for prioritized improvements, including:
- Adding a luxury catering gallery.
- Enhancing the PALETTE CAKE MUSEUM section.
- Connecting the contact form to a backend service.

## Notes for AI Agents
- Focus on maintaining the existing design language: minimal, soft, elegant, and warm.
- Ensure all new features are responsive and work seamlessly across devices.
- When adding new images or sections, ensure they align with the brand's visual identity.

---

For any questions or clarifications, refer to the `README.md` file or consult the project owner.