# The Config File

`_config.yml`

This is the central nervous system to the site.
The config file is not only responsible for creating our development environment, but it also directs jekyll on how to build the `_site/`.

```yml
title: 100 Automations
email: 100Automations@hackforla.org
description: The 100 Automations project showcases Hack for LA automations and microservices that reduce repetitive work in open source development.

```

## SASS Processing

This is how the scss files are processed.
The SASS has a directory it can be found in and a style for processing. 

```yml

sass:
  sass_dir: _sass
  style: compressed

```

## Creating a page for a collection file

Collections are markdown files that contain data.
The collections have an output option that can be set to true.

When output is true, Jekyll will create a new `.html` to replace the collection file in the `_site/`.
Jekyll creates a new url that you can now access the document.

```yml

collections:
  social-media-posts:
    output: true
  memes:
  automations:
  guides:
    output: true
  pages:
    output: true
  bios:
    output: true

```

In order for the site to look uniform we specify the layout for each document.


```yml

defaults:
  - 
    scope:
      path: ""
      type: "guides"
    values:
      layout: "guides"
  - 
    scope:
      path: ""
      type: "pages"
    values:
      layout: "guides"
  - 
    scope:
      path: ""
      type: "bios"
    values:
      layout: "bios"
  - 
    scope:
      path: ""
    values:
      layout: "default"


```
