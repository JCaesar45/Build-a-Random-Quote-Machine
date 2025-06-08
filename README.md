````markdown
# Random Quote Machine

> A frontend project to build a random quote generator app fulfilling FreeCodeCamp’s user stories and tests.

---

## Project Overview

Build a **Random Quote Machine** web app that displays a random quote with its author. The app should allow users to generate new quotes on demand and share them on Twitter.

The project focuses on frontend development using React (or another frontend framework of your choice), fulfilling all required user stories and passing all FreeCodeCamp tests.

---

## Live Demo

[Random Quote Machine Demo](https://random-quote-machine.freecodecamp.rocks/)

---

## User Stories & Requirements

Your app **must** fulfill the following user stories exactly:

1. I can see a wrapper element with a corresponding `id="quote-box"`.
2. Within `#quote-box`, I can see an element with `id="text"` that displays the quote text.
3. Within `#quote-box`, I can see an element with `id="author"` that displays the quote's author.
4. Within `#quote-box`, I can see a clickable element with `id="new-quote"` that triggers fetching a new quote.
5. Within `#quote-box`, I can see a clickable `<a>` element with `id="tweet-quote"` that shares the current quote on Twitter.
6. On first load, the app displays a random quote in the element with `id="text"`.
7. On first load, the app displays the quote's author in the element with `id="author"`.
8. When the `#new-quote` button is clicked, the app fetches and displays a new quote in `#text`.
9. When the `#new-quote` button is clicked, the app fetches and displays the new quote's author in `#author`.
10. The `#tweet-quote` `<a>` element should contain `"twitter.com/intent/tweet"` in its `href` attribute, to tweet the current quote.
11. The `#quote-box` wrapper element should be horizontally centered on the page (tested at 100% zoom, maximized window).

---

## Technologies Allowed / Recommended

- React (recommended for frontend framework)
- HTML5 / CSS3 / JavaScript (ES6+)
- Bootstrap or SASS for styling (optional)
- Redux, jQuery, or vanilla JS (optional, but not necessary)
- External quote APIs or your own quotes data array

⚠️ Note: React 18 has known incompatibilities with the test suite. If using React, consider using React 17 or follow issue guidelines on the FCC repo.

---

## Setup Instructions

### Using CodePen

1. Go to the [CodePen Template](https://codepen.io/freeCodeCamp/full/qRZeGZ).
2. Click **Save** to fork the pen to your account.
3. Build your app by editing HTML, CSS, and JS panes.
4. Add this script tag to your HTML `<body>` to enable FCC tests:

```html
<script src="https://cdn.freecodecamp.org/testable-projects-fcc/v1/bundle.js"></script>
```

5. Run all tests, ensure they pass.
6. Submit your CodePen URL on FreeCodeCamp.

### Using Local Environment

1. Create a React app or vanilla project.
2. Include the test script in your `index.html`:

```html
<script src="https://cdn.freecodecamp.org/testable-projects-fcc/v1/bundle.js"></script>
```

3. Implement all user stories.
4. Open your project in a browser and run the FCC tests.
5. Deploy your project online (GitHub Pages, Netlify, Vercel, etc).
6. Submit the deployed URL on FreeCodeCamp.

---

## Notes & Tips

* For the `#tweet-quote` anchor, use:

```jsx
<a
  id="tweet-quote"
  href={`https://twitter.com/intent/tweet?text=${encodeURIComponent(`"${quote}" - ${author}`)}`}
  target="_blank"
  rel="noopener noreferrer"
>
  Tweet Quote
</a>
```

* Make sure `#quote-box` is centered using CSS (flexbox or grid):

```css
#quote-box {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  margin: auto;
  max-width: 600px;
  padding: 20px;
}
```

* On page load, fetch or select a random quote and display it immediately.
* When `#new-quote` is clicked, update the quote and author.
* Test all features on a maximized browser window at 100% zoom.

---

## License

This project is open source and free to use.

---

Happy Coding! 🚀

---
