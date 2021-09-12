# `_data/`

The data folder exists for holding different data files.
Currently the only data file that is contained within the data folder is called `nav.yml`

```yml
- name: Home
  link: "/"

- name: Press
  link: press-kit/press-kit-index

- name: About
  link: about

- name: Guides
  link: all_guides

- name: Bios
  link: press-kit/all_bios

```

This creates an array of different objects containing a name and link.
The name is arbitrary, but the link is the name of the file that will be displayed.

We access these files using `{{ data.nav }}`.
For example to access `Guides` simply go to  `{{ data.nav[2] }}`.

Then you can target and display the pages name and link using the `name` and `link` properties:
`{{ data.nav[2].name }}` or `{{ data.nav[2].link }}`.
