Urban Spark Electrical - Website

A five-page website for Urban Spark Electrical, a Johannesburg-based residential and commercial electrical services company.
Project

## Pages
1. `index.html` - Home
2. `about.html` - About Us
3. `services.html` - Services
4. `enquiry.html` - Get a Quote
5. `contact.html` - Contact

## Website Goals
- Generate qualified client enquiries.
- Build trust and credibility.
- Provide clear service and contact information.
- Support future SEO and responsive development.

## Target Audience
- Homeowners
- Property developers
- Small and medium-sized businesses

## Organisation
Urban Spark Electrical is a family-owned Johannesburg electrical business with over 15 years of experience and a team of 7 qualified electricians.

Part 2

Pages

| File            | Purpose                                  |
|------------------|-------------------------------------------|
| `index.html`     | Home page - hero, key services, why choose us, testimonials |
| `about.html`     | Company history, mission, vision, team, values |
| `services.html`  | Detailed list of services offered |
| `enquiry.html`   | Quote request form |
| `contact.html`   | Contact details, service area, general enquiry form, map placeholder |
| `style.css`      | Single external stylesheet linked by all pages |

2.Styling approach 

2.1 External stylesheet: all five pages link to one shared `style.css`, using a kebab-case naming convention (e.g. `.site-header`, `.card-grid`, `.hero__image`).
2.2 Reset & base style:a universal box-sizing reset, plus base font, colour and spacing set as CSS custom properties (`:root`) so they're reused consistently across the site.
2.3 Colour scheme: charcoal (`#161b22`), cream background (`#f7f5f0`), amber accent (`#f2a93b`), and teal secondary accent (`#1b8a91`) — chosen to evoke electrical/spark imagery without leaning on a generic template palette.
2.4 Typography: Barlow Condensed for headings (industrial, condensed feel) paired with Inter for body text, set on a modular type scale (`--step--1` to `--step-4`).
2.5 Layout:CSS Grid for the hero section, service card grids, testimonials and footer; Flexbox for the header and navigation.
2.6 Visual styles: `border`, `box-shadow` and background colour used on cards, buttons and form fields, with `:hover`, `:focus`/`:focus-visible` and `:active` states on all interactive elements (nav links, buttons, form inputs).

3.Responsive design

3.1 Breakpoints:
- Desktop:default styles (> 900px)
- Tablet:`@media (max-width: 900px)` - hero and card grids drop to two columns, footer to two columns
- Mobile:`@media (max-width: 600px)` - single-column layout throughout, stacked navigation

3.2 Relative units (`rem`, `em`, `%`, `vw`) are used for spacing, type sizing and widths so the layout scales rather than relying on fixed pixel values. Images use a `sizes` attribute so the browser can pick an appropriately sized image for the current viewport.

3.3 Responsive Images

`about.html`, `services.html` and `contact.html` reference local images under `My images/` (e.g. `My images/image.webp`) 

Changelog

- Created the external `style.css` stylesheet.
- Linked the stylesheet to `index.html`, `about.html`, `services.html`, `enquiry.html` and `contact.html`.
- Reworked page structure with semantic classes for responsive styling.
- Added CSS reset and consistent base styling.
- Added typography hierarchy and responsive font sizing.
- Added Grid and Flexbox layouts.
- Added hover, focus and active states.
- Added tablet and mobile media queries.
- Converted images to responsive HTML using `srcset` and `sizes`.
- Added `<picture>` for the home-page hero image.
- Improved form styling and mobile usability.
- Added accessible navigation with `aria-current="page"`.
- Added this README to document the Part 2 changes and testing requirements.

