# [DOULA NAME] — Death Doula Website

A single-page, production-ready website for a death doula practice. Built with pure HTML, CSS, and vanilla JavaScript — no frameworks, no build tools, no dependencies beyond Google Fonts.

## Quick Start

Open `index.html` in any browser. That's it.

## Customization

### Replace Placeholders

Search and replace these throughout `index.html`:

| Placeholder | Replace With |
|---|---|
| `[DOULA NAME]` | Your business name (uppercase version) |
| `[Doula Name]` | Your business name (title case version) |
| `[FIRST NAME]` | Your first name |
| `hello@placeholder.com` | Your email address |
| `(555) 123-4567` | Your phone number |
| `+15551234567` | Your phone number (tel: format) |

### Add Your Photo

In the About section, find the `<div class="about__photo">` element. Replace the placeholder text with an `<img>` tag:

```html
<div class="about__photo">
  <img src="your-photo.jpg" alt="[FIRST NAME], death doula" style="width:100%;height:100%;object-fit:cover;border-radius:inherit;">
</div>
```

### Update Social Links

Find the `.connect__social` links near the bottom and replace the `href="#"` with your actual profile URLs.

### Connect the Contact Form

The form currently shows a "thank you" message on submit. To make it functional:

- **Formspree**: Change `<form action="#">` to `<form action="https://formspree.io/f/YOUR_ID" method="POST">`
- **Netlify Forms**: Add `netlify` attribute to the `<form>` tag
- **Custom backend**: Update the form action and remove the placeholder JS handler

### Color Palette

All colors are defined as CSS custom properties at the top of the `<style>` block. Adjust any of these to shift the palette:

```css
--color-primary: #B8654A;      /* terracotta */
--color-secondary: #8A9A7B;    /* sage */
--color-dark: #231F1C;         /* warm near-black */
--color-light: #F2EBE1;        /* parchment */
--color-accent: #957B8D;       /* dusty mauve */
--color-gold: #B69B68;         /* antique gold */
```

### Fonts

Fonts are loaded from Google Fonts. To change them, update both the `<link>` tag in the `<head>` and the `--font-display`, `--font-body`, `--font-accent` custom properties.

## Deployment

### GitHub Pages

1. Create a new GitHub repository
2. Push `index.html` (and any images) to the `main` branch
3. Go to **Settings > Pages**
4. Set source to **Deploy from a branch**, select `main`, root `/`
5. Your site will be live at `https://yourusername.github.io/repo-name/`

### Netlify

1. Drag and drop the project folder onto [Netlify Drop](https://app.netlify.com/drop)
2. Connect a custom domain in the Netlify dashboard

### Any Static Host

This is a single HTML file with no build step. Upload it anywhere that serves static files — Vercel, Cloudflare Pages, shared hosting, S3, etc.

## Features

- Fully responsive (mobile-first)
- Smooth scroll navigation
- Scroll-triggered fade-in animations (Intersection Observer)
- Accessible: semantic HTML5, ARIA labels, focus states, proper contrast
- Respects `prefers-reduced-motion`
- Print stylesheet included
- No external images — all visuals are CSS and inline SVG
- Grain texture overlay for warmth and depth
- Handcrafted botanical SVG decorations
- Moon phase timeline illustration

## Browser Support

Works in all modern browsers (Chrome, Firefox, Safari, Edge). The CSS `backdrop-filter` on the nav gracefully degrades in older browsers.

## License

This website was custom-built for [DOULA NAME]. All copy, design, and code are original.
