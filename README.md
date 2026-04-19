# Ebener Santos — Portfolio

Personal portfolio website for Ebener Santos, full-stack developer.

Live at: <!-- TODO: add your live URL here -->

---

## Stack

- HTML5 — semantic structure
- CSS3 — custom design system with CSS variables
- Vanilla JavaScript — i18n, scroll behaviors, form handling
- No frameworks, no build step, no dependencies

---

## Structure

```
my-portfolio/
├── index.html
├── public/
│   ├── css/
│   │   ├── styles.css          # Entry point — imports only
│   │   └── styles/
│   │       ├── tokens.css      # Design tokens (colors, spacing, radius…)
│   │       ├── base.css        # Reset and element defaults
│   │       ├── utilities.css   # Shared layout helpers and reveal animation
│   │       ├── buttons.css     # Button variants
│   │       ├── nav.css         # Fixed header and navigation
│   │       ├── hero.css        # Hero section
│   │       ├── sections.css    # Highlights, About, Stack, Why, Footer
│   │       ├── projects.css    # Featured card and project grid
│   │       ├── forms.css       # Contact section and form fields
│   │       └── responsive.css  # All media queries
│   ├── js/
│   │   └── main.js             # i18n, scroll reveal, nav, form handler
│   └── images/
```

---

## Features

- Multilingual — Portuguese, English, and Spanish with browser auto-detection and localStorage persistence
- Scroll reveal animations via IntersectionObserver
- Active nav link tracking as the user scrolls
- Frosted-glass sticky navigation with scroll state
- Animated hamburger menu with body scroll lock on mobile
- Accessible — semantic HTML, ARIA labels, keyboard navigation, focus-visible states
- Reduced-motion safe — animations respect `prefers-reduced-motion`
- Responsive — mobile-first, tested at 375px and up

---

## Running locally

No build step required. Open `index.html` directly in a browser, or serve with any static file server:

```bash
npx serve .
# or
python3 -m http.server
```

---

## Contact form

The form currently simulates a successful submission. To wire it up for real, replace the placeholder in `public/js/main.js` (marked with a `TODO` comment) with your preferred endpoint — [Formspree](https://formspree.io), Netlify Forms, or EmailJS all work well with a static site.

---

## License

Source code is MIT licensed. See [LICENSE](LICENSE) for details.

Personal content — written copy, profile photo, project screenshots, and the ES monogram — remains the property of Ebener Santos and may not be reproduced without permission.
