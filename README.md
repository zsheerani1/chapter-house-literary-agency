# Chapter House Literary Agency

A static front-end website for a fictional literary agency, built as part of a 
Level 5 Web Application Development diploma project.

## What it does
Provides information about the agency's represented genres, editorial approach, 
and submission guidelines across three pages:
- Home — hero section, represented genres, agency approach
- About — agency background, what the agency looks for, genres of interest
- Submissions — query guidelines and contact form

## Value to users
Authors seeking literary representation can learn about the agency's focus areas, 
understand the submission process, and submit a query directly through the site.

## Technologies used
- HTML5 (semantic elements)
- CSS3 (custom properties, CSS Grid, Flexbox, responsive design)
- Vanilla JavaScript (image slideshow)

## Deployment
Live site: https://zsheerani1.github.io/chapter-house-literary-agency/

## Testing

### Bug: Slideshow image overflowing hero section
**Issue:** The slideshow image was stretching full-width and breaking out of the 
two-column hero layout with no constrained height.  
**Fix:** Removed `aspect-ratio: 4/3` from `.slideshow` and set an explicit 
`height: 420px`. Added `object-fit: cover` to keep images cropped correctly.

### Bug: CSS not applying after upload
**Issue:** Stylesheet appeared uploaded correctly but styling was not rendering 
on the live GitHub Pages site.  
**Fix:** Performed a hard refresh (Cmd+Shift+R) to clear browser cache and 
confirmed the `<link>` tag path matched the exact filename `style.css`.

### Bug: Cards not visually distinct from page background
**Issue:** The four genre cards had the same background colour as the page, 
making them invisible.  
**Fix:** Changed `.card` background to `#ffffff` and darkened the border 
to `#d4cfc8`.

## Credits

### Images
- Hero image 1 (stack of open books): https://unsplash.com/photos/rymh7EZPqRs
- Hero image 2 (wooden bookshelf): https://unsplash.com/photos/NIJuEQw0RKg

### Code
- Slideshow auto-advance logic adapted from MDN Web Docs, setInterval(): https://developer.mozilla.org/en-US/docs/Web/API/setInterval
- classList.add/remove pattern adapted from MDN Web Docs, Element.classList: https://developer.mozilla.org/en-US/docs/Web/API/Element/classList
- Dot navigation pattern adapted from W3Schools, How TO - Slideshow: https://www.w3schools.com/howto/howto_js_slideshow.asp
- CSS Grid layout technique from MDN Web Docs: https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_grid_layout
- Fluid typography using clamp() from CSS-Tricks: https://css-tricks.com/simplified-fluid-typography/
- Box-sizing reset pattern from CSS-Tricks: https://css-tricks.com/box-sizing/
