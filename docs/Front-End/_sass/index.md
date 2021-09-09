# `_sass/`

This folder conatins all of the styles and scss.
This folder is processed using jekyll's built in SASS processor.

This folder is imported into `assets/css` and used to build our _site folder.

## `index.scss`

```scss
@import "variables/index.scss";
@import "components/index.scss";
@import "includes/index.scss";
@import "layouts/index.scss";
@import "press-kit/all_bios.scss";

```

This is the folder directory.
Each folder has a directory that imports all files.

## `components/`

```scss
@import "buttons.scss";
@import "cards.scss";
@import "flexbox.scss";
@import "chips.scss";

```

Each component is stored and categorized in the files show above.
These are components that are mapped out across the site.

To style a component within the site check to see if already exists in the components folder.
Then use the class name in the html of your component and style.

## `includes/`

```scss
@import "About/index.scss";
@import "All-Guides/index.scss";
@import "Default/index.scss";
@import "Home/index.scss";
@import "Press/index.scss";

```

Includes are first organized by the page that the include exists on.
When you style a page you use includes to componentize each section of the page.

Each page is built using includes and those includes contain styles for:

* Typography
* Spacing
* Layout
* Color

## `layouts/`

```scss
@import 'guides_hero.scss';
@import 'guides.scss';

```

This example above is for styling each guide.
Each guide is displayed using the `_layouts/guides.html`.

The layouts are directly correlated to the layouts folder.
Currently the layouts that are being used are guides.

## `press-kitstyle`

Press-kit is a folder located in the root of the site.
This folder contains the different sections of the Press Kit Page.

This folder is for styling the subpages of the press-kit page.

## `variables/`

```scss
@import "colors.scss";
@import "typography.scss";

```

Variables are used to create a shorthand expression in place of the css code for colors and typography.
