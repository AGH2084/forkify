# Repository Guidelines

## Project Structure & Module Organization

`index.html` is the Parcel entry point. Application code lives in `src/js/`: `model.js` handles recipe data and state, `controller.js` coordinates actions, `helpers.js` and `config.js` provide shared utilities and settings, and `views/` contains UI components. Styles are in `src/sass/`, with `main.scss` importing partials. Put images and icons in `src/img/`. `dist/` and `.parcel-cache/` are generated outputs; do not edit them by hand.

## Build, Test, and Development Commands

Run `npm install` to install dependencies.

- `npm run start` launches Parcel’s development server for `index.html` (normally at `http://localhost:1234`).
- `npm run build` creates a production bundle in `dist/`.

There is no configured automated test or lint command. For UI changes, run the development server and check the affected flows in a browser; run the production build to catch bundling errors.

## Coding Style & Naming Conventions

Use the existing ES module style and keep responsibilities aligned with the current model/controller/view structure. JavaScript and SCSS use two-space indentation. Follow `.prettierrc`: use single quotes and omit parentheses around a single arrow-function parameter. Use descriptive camelCase names for JavaScript modules, functions, and variables; SCSS partials use the existing underscore-prefixed naming pattern (for example, `_recipe.scss`). Keep view-specific markup and behavior in the relevant `src/js/views/` module.

## Testing Guidelines

No test framework or coverage requirement is configured. When adding tests, first document the chosen runner and its command in `package.json`; name test files after the module or behavior they cover. Until then, verify changes manually with `npm run start` and `npm run build`.

## Commit & Pull Request Guidelines

Recent history uses short, informal subjects and does not establish a strict convention. Write concise imperative commit subjects, such as `Fix recipe pagination`. Pull requests should explain the user-visible change, note relevant manual checks, link related issues when available, and include screenshots for visual changes.

## Security & Configuration

Keep API credentials and local secrets out of source control. Store environment-specific configuration outside committed files and avoid including credentials in screenshots or logs.
