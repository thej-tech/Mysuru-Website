<<<<<<< HEAD
# Mysuru-Website
=======
# Mysuru Website — Concepts Used

## HTML

### Document structure and metadata
Each page uses the HTML5 document declaration and sets its language with `lang="en"`. The `<head>` contains character encoding, a responsive viewport setting, a page title, a description for search previews, and a link to the shared stylesheet.

### Semantic page layout
Elements such as `<header>`, `<nav>`, `<main>`, `<section>`, `<article>` and `<footer>` give page content meaningful structure. This makes the pages easier for browsers, assistive technology and people reading the markup to understand.

### Headings and text
Headings from `<h1>` to `<h3>` organize each page into a clear content hierarchy, while paragraphs hold descriptive text. `<strong>` marks important names and ideas so they receive emphasis and stand out to readers.

### Links and navigation
The navigation list connects the home, legacy, places, culture and hotels pages using relative links. The `aria-current="page"` attribute identifies the current page, while in-page links such as the skip link provide a shortcut to the main content.

### Images and accessibility
Images use descriptive `alt` text so their subject is available when an image cannot be seen or loaded; hotel photos also use `loading="lazy"` to defer loading until needed. Hotel image captions link to their Pexels sources, and the page clarifies that those representative interiors are not confirmed photos of the named hotels.

### Lists, cards and tables
Unordered lists present navigation and additional attractions, and `<article>` elements group related destination, culture or hotel information into cards. The hotels page uses a captioned table with `<thead>`, `<tbody>`, `<th>` and `<td>` to compare types of stays.

### Special attributes and entities
The pages use `id` values for in-page targets and CSS hooks, and `class` values to apply page-specific themes. Attributes such as `target`, `rel`, `loading` and `aria-current`, plus encoded characters such as `&amp;`, support safe links, image loading, accessibility and valid markup.

## CSS

### External stylesheet and shared design tokens
All pages load the same `style.css`, so common layout and visual rules stay consistent across the site. The `:root` custom properties define reusable colors, spacing, corner radii, shadows and transition timing.

### Page-specific themes
Each page's body class sets its own background, card wash and divider colors, such as `.page-legacy` or `.page-culture`. The shared components use those variables, giving every page a distinct color identity without duplicating the overall design.

### Reset and box model
The universal selector and its pseudo-elements set `box-sizing: border-box`, making element dimensions easier to predict. The body rule removes the browser's default margin and sets the site's base font, line height, text color and themed background.

### Selectors and reusable component styles
Element selectors style common HTML elements, while class selectors, IDs and attribute selectors target specific page components and navigation states. Shared rules style headings, links, images, headers, sections, cards, status labels, tables and footers consistently.

### Typography and responsive sizing
Font weights, line heights, readable maximum text widths and `clamp()` help headings adapt to different screen sizes. Muted text and accent colors create visual hierarchy, while bold text receives a consistent accent color.

### Layout with Flexbox and Grid
Flexbox lets the navigation links wrap when space is limited. CSS Grid arranges content cards and image-and-text sections into columns that adapt to the available width.

### Spacing, borders and visual depth
Padding, margins and gaps separate content and make it easier to scan. Borders, rounded corners and subtle shadows distinguish cards, tables and images from each page's background.

### Images and tables
Images are constrained to their containers, and `object-fit: cover` crops card images consistently. Tables use collapsed borders and a horizontally scrollable wrapper so comparison data remains usable on narrow screens.

### Hover, focus and accessibility
Transitions and hover styles provide feedback on links, cards and list items; the active navigation item stays visibly highlighted for the current page. `:focus-visible` adds a clear outline for keyboard users, and the skip link becomes visible when focused.

### Responsive media query
The `@media (max-width: 768px)` rules adjust spacing and heading sizes for smaller screens. They also stack the about section and simplify selected grids and table spacing for mobile layouts.
>>>>>>> 2682a74 (Add Mysuru website)
