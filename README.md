# MsVsPrints Website

A clean, minimal static website for msvsprints.com.au

## Folder Structure

```
msvsprints/
├── index.html          ← Homepage
├── style.css           ← All styles (one file for the whole site)
├── images/             ← Put ALL your photos here
│   └── (add your images here)
└── pages/
    ├── about.html
    ├── gallery.html
    └── contact.html
```

## Adding Your Images

1. Copy your photos into the `images/` folder
2. In `index.html`, find the comment `<!-- Replace this div with:` and swap in your image tag
3. Same for `pages/about.html` and `pages/gallery.html`

Example:
```html
<!-- BEFORE -->
<div class="hero-placeholder"><span>Add your hero image here</span></div>

<!-- AFTER -->
<img src="images/hero.jpg" alt="MsVsPrints" />
```

## Setting Up the Contact Form

1. Go to https://formspree.io and create a free account
2. Create a new form — they'll give you an ID like `xpzgkwqr`
3. In `pages/contact.html`, replace `YOUR_FORM_ID` with your actual ID
4. Done — form submissions go straight to your email

## Deploying to Netlify

1. Push this folder to GitHub
2. Log into netlify.com → Add new site → Import from GitHub
3. Select your repo → Deploy
4. Add your custom domain in Site Settings → Domain Management

## Making Updates (the workflow)

1. Edit files in VS Code
2. Open `index.html` in your browser to preview
3. When happy: `git add . && git commit -m "describe your change" && git push`
4. Netlify auto-deploys in ~30 seconds ✅
