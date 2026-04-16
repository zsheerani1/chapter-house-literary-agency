# Chapter House Literary Agency

A static front-end website for a fictional literary agency, built as part of a Level 5 Diploma in Web Application Development at Code Institute.

Live site: https://zsheerani1.github.io/chapter-house-literary-agency/

---

## Contents

- [Project Overview](#project-overview)
- [User Stories](#user-stories)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Wireframes](#wireframes)
- [Deployment](#deployment)
- [Testing](#testing)
- [Credits](#credits)

---

## Project Overview

Chapter House Literary Agency is a three-page website for a fictional literary agency. It was built using HTML5, CSS3, and a CSS animation for the image slideshow.

The site is aimed at authors looking for literary representation. It tells them what the agency looks for, which genres it represents, and how to submit a query.

---

## User Stories

As an author seeking representation, I want to quickly understand what genres the agency represents, so I can decide whether my manuscript is a good fit before investing time in a query.

As a first-time querier, I want clear submission guidelines that tell me exactly what to include and how to format my submission, so I do not make mistakes that could hurt my chances.

As a writer researching agents, I want to learn about the agency's editorial approach and values, so I can assess whether their working style suits me.

As a returning visitor, I want to be able to navigate quickly between pages, so I can find the specific information I need without scrolling through the whole site.

As a user on a mobile device, I want the site to work cleanly on my phone, so I can research the agency and access submission information on the go.

---

## Features

- Sticky navigation header with active page indicator on all three pages
- Hero section with a pure CSS auto-advancing image slideshow
- Four-column genre cards on the home and about pages
- Fully responsive layout using CSS Grid and Flexbox across four breakpoints
- Submission contact form with labelled inputs and visible focus states
- Consistent header and footer across all pages

---

## Technologies Used

- HTML5
- CSS3 including Grid, Flexbox, custom properties, clamp() for fluid typography, and keyframe animation
- Git and GitHub for version control
- GitHub Pages for deployment

---

## Wireframes

[Add Figma wireframe screenshots here]

---

## Deployment

The site was deployed to GitHub Pages using the following steps:

1. All project files were pushed to the main branch on GitHub
2. In the repository, went to Settings then Pages
3. Under Source, selected the main branch and saved
4. GitHub Pages built and published the site automatically

To clone and run the project locally:

1. Go to https://github.com/zsheerani1/chapter-house-literary-agency
2. Click the green Code button and copy the HTTPS URL
3. In your terminal run git clone https://github.com/zsheerani1/chapter-house-literary-agency.git
4. Open index.html directly in a browser — no build tools or installation needed

---

## Testing

### Manual Testing

Feature: Home nav link — Goes to index.html — Pass
Feature: About nav link — Goes to about.html — Pass
Feature: Submissions nav link — Goes to submissions.html — Pass
Feature: Active nav state — Current page link underlined — Pass
Feature: Slideshow — Image changes without interaction — Pass
Feature: Card hover — Card raises with shadow — Pass
Feature: Form submit — Form submits on button click — Pass
Feature: Layout at 375px — Content stacks to one column — Pass
Feature: Cards at 650px — Cards go to two columns — Pass
Feature: Footer — Visible and consistent on all pages — Pass

### Browser Compatibility

Tested and working on Google Chrome, Safari, and Firefox.

### Responsiveness

Tested at 360px, 375px, 768px, and 1280px. The layout adjusts correctly at each breakpoint. The hero section moves from single column on mobile to two columns on desktop. Cards move from one column on mobile to two on tablet and four on desktop.

### Validator Testing

- HTML: Tested using the W3C HTML Validator at https://validator.w3.org/
- CSS: Tested using the W3C CSS Validator at https://jigsaw.w3.org/css-validator/

### Lighthouse



### Bugs

**Slideshow image overflowing the hero section**
The slideshow image was stretching full width and breaking out of the two-column hero layout. The container had no constrained height. Fixed by removing aspect-ratio from the slideshow container and setting an explicit height of 420px, with object-fit cover on the images to keep them cropped correctly.

**CSS not applying after upload**
After pushing the stylesheet to GitHub, the styling was not rendering on the live site. The browser was serving a cached version. Fixed by performing a hard refresh to force the browser to load the latest files.

**Genre cards not visible**
The four genre cards had the same background colour as the page, making them invisible. Fixed by setting the card background to white and darkening the border colour.

**Slideshow track bars appearing outside container**
After switching from JavaScript to a pure CSS animation, two horizontal bars appeared below the slideshow. These were the slides track div rendering outside the container. Fixed by adding overflow hidden to both the slideshow and hero layout containers.

---

## Credits

### Images

- Hero image 1, stack of open books: https://unsplash.com/photos/rymh7EZPqRs
- Hero image 2, wooden bookshelf: https://unsplash.com/photos/NIJuEQw0RKg

Both images are free to use under the Unsplash Licence: https://unsplash.com/license

### Code

