# މަކްތަބާ އަޘަރިއްޔާ — Official Social Media Portal

A modern, responsive Dhivehi single-page website for **މަކްތަބާ އަޘަރިއްޔާ**. The website acts as an official portal for the foundation's social media channels across Telegram, Facebook, and X.

The project is built entirely with **HTML and CSS**, with no frameworks or JavaScript dependencies.

## Features

- Fully responsive desktop, tablet, and mobile layout
- Right-to-left Dhivehi interface
- Local Dhivehi typography using Maumoon and Faseyha
- Official foundation logo in the header and footer
- High-resolution Islamic mosque cover image
- Telegram, Facebook, and X social-media sections
- Multiple editable links under each platform
- CSS-only light and dark mode toggle
- Animated skeleton loading screen
- Smooth scrolling and scroll-triggered reveal animations
- Modern card and navigation hover effects
- Reduced-motion accessibility support
- SEO title, description, theme color, and viewport metadata
- No build tools or external code libraries required

## Fonts

The website uses two locally hosted Dhivehi fonts:

- **Maumoon** — main headings and subheadings
- **Faseyha** — paragraphs, navigation, labels, and supporting text

The font files are stored in `assets/fonts/` and loaded through `@font-face` rules in `styles.css`.

## Project Structure

```text
landingpage/
├── index.html
├── styles.css
├── README.md
└── assets/
    ├── fonts/
    │   ├── Maumoon.otf
    │   └── Faseyha.ttf
    └── images/
        ├── foundation-logo.jpg
        └── islamic-cover.jpg
```

## Running Locally

No installation or compilation is required. Download or clone the project and open `index.html` in a modern web browser.

You can also serve the folder through any static web server:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Customization

### Social-media links

Open `index.html` and replace the placeholder `href="#"` values inside the Telegram, Facebook, and X cards with the foundation's official URLs.

```html
<a href="https://example.com">މައި ޗެނަލް</a>
```

### Text content

All Dhivehi headings, descriptions, organization details, and footer content can be edited directly in `index.html`.

### Logo and cover image

- Replace `assets/images/foundation-logo.jpg` to update the foundation logo.
- Replace `assets/images/islamic-cover.jpg` to update the hero cover.

Keeping the same filenames means no CSS or HTML changes are necessary.

### Colors

The main color palette is controlled by CSS custom properties at the beginning of `styles.css`:

```css
:root {
  --ink: #073d35;
  --deep: #052e29;
  --green: #0b564b;
  --cream: #f7f4eb;
  --gold: #c89f55;
}
```

## Browser Support

The core layout, dark mode, skeleton loader, and hover effects work in modern browsers. Scroll-driven reveal animations use modern CSS scroll timelines and progressively fall back to a fully visible page in browsers that do not support them.

## Image Credit

The placeholder mosque cover photograph is sourced from [Unsplash](https://unsplash.com/photos/the-inside-of-a-large-building-with-a-domed-ceiling-BqJShRC-WF4). Replace it with an approved foundation image before the final public launch if required.

## License

The foundation's name, logo, Dhivehi content, and supplied brand assets remain the property of their respective owner. Add your preferred software license before redistributing the project.

