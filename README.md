
# FreshBite — F&B Online Shop (HTML5 + CSS3)

This is a minimal, responsive front-end project with 4 pages and a shared header/footer.

## File Structure
/fnb-shop
│── /assets
│   ├── /images
│   ├── /icons
│── /css
│   ├── style.css
│── index.html
│── products.html
│── about.html
│── contact.html

## How to run
Just open `index.html` in your browser (no build needed).

## Bonus: Deploy on Heroku (Static)
Heroku isn’t a static host by default. Use the “heroku-buildpack-static” and add a `static.json` file:

1) Create app:
```
heroku create freshbite-fnb
heroku buildpacks:add https://github.com/heroku/heroku-buildpack-static
```

2) Add `static.json`:
```
{ "root": ".", "headers": { "/**": { "Access-Control-Allow-Origin": "*" } } }
```

3) Commit and push:
```
git init
git add .
git commit -m "FreshBite initial"
git push heroku main
```

Alternatively, deploy on Netlify / Vercel which are simpler for static sites.
