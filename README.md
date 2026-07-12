# WebStudio

An educational single-page website created as part of the GoIT HTML and CSS
homework assignment. This version is updated for `goit-markup-hw-03` and builds
the WebStudio layout with semantic HTML, CSS, and Flexbox.

## Implemented Sections

- Header with logo, navigation, and contact information
- Hero section with centered title and action button
- Features section with visually hidden heading
- Team section with four profile cards
- Portfolio section with six project cards
- Footer with logo and description

## Technologies

- HTML5
- CSS3
- Flexbox
- Modern Normalize
- Google Fonts: Roboto and Raleway

## Layout Details

- The page uses a reusable `.container` with a 1158px max-width and 15px side
  padding.
- Shared section spacing is handled by the `.section` utility class.
- Flex layouts use `gap` for spacing instead of right margins.
- Feature, team, and portfolio card widths are calculated with `calc()`.
- The portfolio card border is applied only on the left, right, and bottom
  sides, as required by the homework criteria.
- The project does not use JavaScript, CSS Grid, floats, inline styles,
  `!important`, decorative shadows, or fixed section heights.

## Project Structure

```text
.
├── css/
│   ├── common.css
│   ├── features.css
│   ├── footer.css
│   ├── header.css
│   ├── hero.css
│   ├── main.css
│   ├── portfolio.css
│   └── team.css
├── images/
│   ├── portfolio-1.jpg
│   ├── ...
│   └── team-4.jpg
├── index.html
└── README.md
```

Only `css/main.css` is linked in `index.html`. It imports the separate
stylesheets for each page section.

## Getting Started

Open `index.html` in a browser. No dependency installation or build step is
required.

## Checks

- `modern-normalize` is connected before the local stylesheet.
- `git diff --check` passes without whitespace issues.
- Local static checks confirm that there are no scripts, inline styles, CSS
  Grid, floats, `!important`, decorative shadows, or layout `margin-right`
  usage.
- The only fixed `height` values are the required image reset
  (`height: auto`) and the `.sr-only` accessibility helper.
- All images are stored locally in JPG format.
