# `_includes/`

## `Home/`

`index.html`:

```html
{% include Home/action.html %}
{% include Home/wave.html %}
{% include Home/ato_grid.html %}
{% include Home/border.html %}
{% include Home/guide_grid.html %}

```

The Home page is our most populous page containing three sections and a divider component.
The divider is called `wave.html`.

`border.html` is a section containing three separate user experiences.

## `About/`

`index.html`:

```html
{% include About/about_one.html %}
{% include About/join_us.html %}
{% include About/acknowledgements.html %}

```

As you can see from the index file this page is built using three components.
The order in which we use our include statement is the order that these files are displayed on our page.

1. `about_one.html`

_Image of the about 100 Automations section_

## `Press/`

`index.html`:

```html
{% include Press/press_action.html %}
{% include Press/wave.html %}
{% include Press/share_ato.html %}

```

This is the press page which only has two sections for content.
If you notice, there is also a `wave.html`: just like the home page.

The `press_action.html` is a page that contains all the links to navigate the `press-kit/`

## `All-Guides/`

`index.html`:

```html
{% include All-Guides/all_guides_hero.html %}
{% include All-Guides/all_guides_list.html %}

```

As you can see from the index file this page is built using two components.
The order in which we use our include statement is the order that these files are displayed on our page.

## `toc.html`

This file is located in the includes and belongs to the guide layuout.
In read the markdown file that is being processed through jekyll we include toc.html

`toc.html` captures the jekyll variables and creates an html nav item list.
