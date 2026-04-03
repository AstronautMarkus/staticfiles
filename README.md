# staticfiles

CDN-like personal repository for public static assets, hosted via **GitHub Pages**.

## Live URL

```
https://astronautmarkus.github.io/staticfiles/
```

## Structure

```
staticfiles/
├── index.html          # CDN landing page (browse & copy URLs)
├── css/
│   └── styles.css      # Page stylesheet
└── assets/
    ├── icons/          # Icon images (PNG, SVG, WebP, …)
    └── profile/        # Profile pictures (JPG, PNG, WebP, …)
```

## How to add a new asset

1. Drop the image file into the appropriate folder:
   - **Icons** → `assets/icons/`
   - **Profile pictures** → `assets/profile/`
2. Open `index.html` and add an entry to the `ASSETS` array near the bottom of the file:
   ```js
   { section: "icons",   file: "logo.png"   },
   { section: "profile", file: "avatar.jpg" },
   ```
3. Commit and push — GitHub Pages will serve the file within seconds.

### Direct URL format

```
https://astronautmarkus.github.io/staticfiles/assets/<section>/<filename>
```

Example:
```
https://astronautmarkus.github.io/staticfiles/assets/icons/logo.png
https://astronautmarkus.github.io/staticfiles/assets/profile/avatar.jpg
```

## GitHub Pages setup

1. Go to **Settings → Pages** in this repository.
2. Set the source to the `main` branch, root folder (`/`).
3. Save — the site will be available at the URL above.
