# css_frameworks

**Bootstrap 5 + Webpack setup exercise** — configuring a modern front-end build pipeline from scratch, based on Bootstrap's official Webpack guide.

## What it covers

- Webpack configuration: entry/output, dev server with hot reload, HtmlWebpackPlugin
- Full SCSS pipeline: `sass-loader` → PostCSS with Autoprefixer → `css-loader` → `MiniCssExtractPlugin`
- Importing Bootstrap's SCSS and JS (full bundle and selective plugin imports)
- Asset handling for inline SVG icons

## Tech stack

- Bootstrap 5
- Webpack 5 (webpack-dev-server, html-webpack-plugin, mini-css-extract-plugin)
- Sass/SCSS, PostCSS, Autoprefixer

## Run it

```
npm install
npx webpack serve
```

Then open http://localhost:8080 — the page hot-reloads on changes to `src/`.

Build for production output in `dist/`:

```
npx webpack
```

## Structure

```
├── src/
│   ├── index.html       # page template
│   ├── js/main.js       # entry point, imports SCSS + Bootstrap JS
│   └── scss/styles.scss # custom styles importing Bootstrap SCSS
└── webpack.config.js    # build pipeline configuration
```
