# 📄 Simple Lightbox

Build an image gallery where users click a thumbnail to see a larger version of the image in
a lightbox.

## 🎯 Overview

A **gallery** is a group of images arranged in a clean, organized layout. A **lightbox** is a
large image overlay that appears on top of the page when an image is clicked. You see them all
the time on real websites: portfolios, product pages, travel sites, and photography sites.

This exercise brings together several important ideas:

- **HTML** creates the page structure: the gallery and the hidden lightbox
- **CSS** controls the layout and appearance: a CSS Grid gallery, polished thumbnails, and a
  full-screen overlay
- **JavaScript** adds the click behavior that opens and closes the lightbox

**You are not expected to learn JavaScript in this assignment.** The JavaScript is already
written for you. Your job is to understand what the code does and how it connects to the HTML
and CSS you have already learned.

> [!IMPORTANT]
> **The companion videos for this exercise are in Canvas**, on the assignment page. They
> walk you through every step, so watch them there instead of working from this file
> alone.

## 🧠 What You Will Learn

By completing this exercise, you will practice how to:

- Build a gallery layout with **CSS Grid** (`display: grid`, `grid-template-columns`, `gap`)
- Style images so they look clean and clickable, including a smooth hover effect with
  `transition` and `transform`
- Use `position: fixed` to build an overlay that covers the whole browser window
- Center content inside the overlay with Flexbox
- Link a JavaScript file to an HTML page
- Read basic JavaScript and explain what it does: selecting elements, listening for clicks,
  and changing an element's `src`, `alt`, and `display`

## 🎬 Watch the Videos in Canvas and Follow Along

The screencast videos are on this assignment's page in **Canvas**, not in this repo. They
walk you through the entire exercise. Watch them **in order** and follow along in your code
editor. Pause whenever you need time to finish a step — it is normal to pause, rewind, and
rewatch parts of a coding demonstration.

Each video builds on the previous one, so please don't skip ahead.

| Video | What you will do |
| --- | --- |
| **Part 1 — HTML** | Add the gallery of thumbnail images and build out the hidden lightbox: the content box, the close button, and the empty image that JavaScript fills in. |
| **Part 2 — CSS** | Turn the gallery into a three-column grid, style the thumbnails and their hover effect, and hide the lightbox until it's needed. |
| **Part 3 — JavaScript** | Link `lightbox.js` to the page and walk through the code to see how it opens and closes the lightbox. You are not required to write any JavaScript. |

> [!IMPORTANT]
> **A few steps in this repo are different from the videos.** Follow the videos for the
> code, and follow this repo for getting your files and submitting:
>
> - **Getting the starter files:** don't download a ZIP from GitHub. Create your own repo
>   from this template and open it with GitHub Desktop, as described in the
>   [README](README.md#-getting-started).
> - **Submitting:** don't zip your folder or upload a file. Publish your page to GitHub
>   Pages and submit a pull request URL in Canvas, as described in the
>   [README](README.md#-submitting-the-assignment).

## 📂 Starter Files

| File / Folder | Purpose |
| --- | --- |
| `index.html` | The page. It has the header, footer, and an empty lightbox `section`. You add the gallery and the lightbox's inner content. |
| `lightbox.css` | The styles. Some properties are written for you; comments mark the empty spots where you add the rest. |
| `lightbox.js` | The JavaScript that opens and closes the lightbox. **It's already finished** — you only need to link it in `index.html`. |
| `reset.css` | Removes default browser styles so the page looks the same everywhere. Don't edit it. |
| `images/` | The gallery images: `smpte.jpg`, `indian.jpg`, `bbc.jpg`, and `circle.jpg`. |

Watch for the names the JavaScript depends on. If any of these are misspelled in your HTML,
the lightbox won't work:

| Name | Used on |
| --- | --- |
| `class="thumbnail"` | Every gallery image |
| `id="lightbox"` | The lightbox `section` (already in the starter file) |
| `id="lightbox-img"` | The large image inside the lightbox |
| `id="close-btn"` | The close button |

## ✅ Before You Submit

Check the following:

- [ ] The gallery images are inside an element with the class `gallery`
- [ ] Every gallery image has the class `thumbnail` and useful `alt` text
- [ ] The gallery displays as a three-column grid with space between the images
- [ ] The gallery switches to one column on small screens (narrow your browser to check)
- [ ] The thumbnails fill their grid columns and enlarge slightly and smoothly on hover
- [ ] The lightbox is hidden when the page first loads
- [ ] The lightbox contains a `.lightbox-content` box, a close button, and the `#lightbox-img` image
- [ ] `lightbox.js` is linked in `index.html`
- [ ] Clicking a thumbnail opens the lightbox with the matching large image
- [ ] Clicking the **X** button closes the lightbox
- [ ] Clicking the dark background closes the lightbox
- [ ] You saved all of your files
- [ ] The page is live on GitHub Pages and the URL is in your pull request

## 🧮 Grading

| Criteria | Points |
| --- | --- |
| **Gallery HTML** — gallery container with all thumbnail images, each with the `thumbnail` class and useful `alt` text | 2 |
| **Lightbox HTML** — content box, close button, and lightbox image with the correct IDs and classes | 2 |
| **Gallery CSS** — three-column grid with a gap, thumbnails fill their columns, smooth hover effect | 2 |
| **Lightbox CSS** — lightbox hidden by default and covers the page as a centered overlay when open | 1 |
| **JavaScript** — `lightbox.js` linked; the lightbox opens with the right image and closes from the **X** and the background | 2 |
| **Submission** — page live on GitHub Pages, pull request open with the template filled in | 1 |
| **Total** | **10** |

## 🛠️ Troubleshooting

If something is not working, check these common issues first:

- Did you save every file?
- Are the class names and IDs spelled exactly right — `thumbnail`, `lightbox-img`,
  `close-btn`? Capitalization counts.
- Are the image paths correct, including the `images/` folder, like `images/bbc.jpg`?
- Is the `script` element linking `lightbox.js` spelled correctly, and does the file name
  match?
- Does clicking a thumbnail do nothing? Open your browser's developer tools
  (<kbd>F12</kbd> or <kbd>Cmd</kbd> + <kbd>Option</kbd> + <kbd>I</kbd>) and look in the
  **Console** for a red error message.
- Is the grid uneven? Gallery images should all be the same dimensions.
- Are you missing a semicolon, bracket, or closing tag?

**Having problems with the videos?**

- **Getting a warning about third-party cookies?** Try using Chrome. Safari's default
  security settings may prevent embedded Canvas videos from playing unless those settings
  are changed.
- **Getting an "Access Denied" error?** Refresh your browser. In many cases, the videos
  will load correctly after the page reloads.

## 💡 Optional Ideas

If you finish early and want to experiment, try:

- Adding more images to the gallery
- Changing the number of columns
- Adjusting the hover effect
- Styling the lightbox differently
- Adding captions below the images

If your final project includes multiple images, this is a feature you may be able to adapt
and reuse. Focus on understanding how the pieces work together rather than memorizing the
code.

## 📚 Resources

- [MDN — Basic concepts of grid layout](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_grid_layout/Basic_concepts_of_grid_layout)
- [MDN — `position`](https://developer.mozilla.org/en-US/docs/Web/CSS/position)
- [MDN — Using CSS transitions](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_transitions/Using_CSS_transitions)
- [MDN — `<script>`: The Script element](https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/script)
- [MDN — `addEventListener()`](https://developer.mozilla.org/en-US/docs/Web/API/EventTarget/addEventListener)

---

The AI policy and submission instructions are in the [README](README.md).
