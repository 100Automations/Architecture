# Site Components for 100 Automations

Split between Front-End (UI and UX: HTML, SASS, Etc.) and Back-end (Programming and Data: Ruby)

## Front-End

The "Front-End" of our site will be defined by the HTML and CSS we create.
We will be processing the Front-End using Jekyll.

Jekyll has it's own SASS processor that we will be using.
All styles can be found in the [_sass/](Front-End/_sass/index.md) section of this document.

### _HTML displaying our site_

The HTML is responsible for displaying the site. The way a page is displayed is ranked in order:

1. Front Matter: This is where data is contained in the page.
2. Liquid: This is usually responsibly for querying the data.
3. HTML: The text that this document holds for display.
4. Javascript: Responsible for UI, UX.

Liquid will help with processing our back-end elements for display.
The HTML is responsible for all page building elements and for containing liquid.

Javascript is used within the site to help execute User Experiences.
Javascript can also contain back-end elements using liquid.

#### `_includes/`

An "include" component is a section of each page within our site.
Each include folder contains several different files and an `index.html`.

`index.html` is the root directory for each folder and establishes how the page is built.
The folders represent each page:

* About
* All-Guides
* Default
* Home
* Press

There is also a file called `toc.html`.

#### `_layouts/`

This folder contains the layouts of each page that is in the site.
Layouts are different from includes, and define the layout of a collection's output.

### _Sass Styles_

Jekyll has it's own Sass processor, and this is defined in our [config.yml](docs/../Back-End/config/index.md).
The [_sass](Front-End/_sass/index.md) will be imported into the site's `assests/css/`.

## Back-End

The "Back-End" is written in Ruby, and this means that your liquid objects are processed by jekyll first.
Jekyll will process the liquid on a `.html` before the HTML text.

The same goes for any documents written in Ruby: All `.yml` processed first.
These documents are considered the "Back-End" of the site, and are located not only in liquid but in the front matter as well

### _Ruby_

Ruby is responsible for holding and querying data:

* Automations
* Guides
* Team Bios
* Memes
* Social Media Posts

Ruby also establishes routing; processes SASS; Builds the site.
This is being done with Jekyll.

#### `_data/`

This is used for establishing routing for the different components on the site.
