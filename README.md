# Your Name — Personal Website

A clean, minimalistic one-page personal website (plain HTML/CSS/JS) with a
separate blog page, built to be hosted for free on **GitHub Pages**.

## Files

```
.
├── index.html   → the main one-page site (hero, about, projects, contact)
├── blog.html    → simple blog page (empty by default, template included)
├── style.css    → all styling + theme colors (one file, clearly commented)
├── script.js    → tiny bit of JS (mobile menu + footer year)
└── README.md    → this file
```

## 1. Customize the content

- **Text**: open `index.html` and `blog.html` and replace placeholder text
  (name, tagline, bio, project descriptions, email, social links).
- **Images**: every image is a stock placeholder wrapped in comment markers:

  ```html
  <!-- **************** IMAGE START **************** -->
  <img src="..." alt="...">
  <!-- **************** IMAGE END **************** -->
  ```

  Search those markers in `index.html` and swap the `src` for your own
  photos/screenshots (e.g. upload an `images/` folder to the repo and point
  `src` to `images/your-photo.jpg`).

- **Colors/theme**: open `style.css` and look for:

  ```css
  /* **************** THEME START **************** */
  :root { ... }
  /* **************** THEME END **************** */
  ```

  Every color used across the whole site is defined once in that block —
  change a value there and it updates everywhere.

- **Blog posts**: `blog.html` contains a commented example `blog-post` block
  with instructions right above it. Copy it, uncomment it, and fill in your
  own title/date/text each time you want to publish a post.

## 2. Put it on GitHub Pages

1. Create a new GitHub repository (public).
   - If the repo is named `yourusername.github.io`, the site will be live at
     `https://yourusername.github.io/`.
   - Any other repo name works too — the site will live at
     `https://yourusername.github.io/repo-name/`.
2. Upload these files (`index.html`, `blog.html`, `style.css`, `script.js`)
   to the root of that repository (via the GitHub web UI, or `git push`).
3. In the repo, go to **Settings → Pages**.
4. Under **Build and deployment → Source**, choose **Deploy from a branch**.
5. Under **Branch**, choose `main` (or `master`) and folder `/ (root)`, then
   **Save**.
6. Wait a minute or two — GitHub will give you a live URL at the top of the
   Pages settings screen.

That's it — no build step, no dependencies to install.

## Notes

- Fonts (Sora + Inter) load from Google Fonts via a `<link>` tag in the
  `<head>` — no installation needed, works automatically on GitHub Pages.
- The site is fully responsive and includes a mobile menu toggle.
- Keyboard focus states and `prefers-reduced-motion` are respected for
  accessibility.
