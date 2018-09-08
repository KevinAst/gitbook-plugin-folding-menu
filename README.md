# gitbook-plugin-folding-menu

This gitbook plugin **manages large left-nav menus** by **visualizing only
one section at a time** _(the active section)_.

<!--- Badges for CI Builds ---> 

[![NPM Version Badge](https://img.shields.io/npm/v/gitbook-plugin-folding-menu.svg)](https://www.npmjs.com/package/gitbook-plugin-folding-menu)

## Overview

The high-level points of interest are:

- On initial display, only the top-level menu items are displayed.

- Navigating to a section with sub-content will dynamically expand it,
  collapsing any prior section.

- The active section will expose the entire sub-menu depth _(i.e. all
  it's ancestry, not just direct children)_.

- Navigating between sections continues to expand only the active
  section _(expanding the active section while collapsing any section
  previously expanded)_.

- **Animation is used** to make the user experience more intuitive
  _(i.e. they can visually see what is happening)_!

- Sections that are composed of multiple pages are supported.

This plugin has the effect of "taming" a big unruly menu structure, by
exposing only one section at a time, making it more intuitive for
end-user consumption.

You can **see this in action** at: https://feature-u.js.org/ _(one of
my open source projects)_.

This project is a significant improvement on other similar plugins.

## Install

- Add the `"folding-menu"` plugin to your **book.json** file:

  ```js
  {
    "plugins": [
      ... other plugins you may be using
      "folding-menu"
    ]
  }
  ```

- For https://legacy.gitbook.com/ usage, plugins are automatically installed.

- For local gitbook usage run `gitbook install` to install and prepare
  all plugins for your books:

  ```shell
  gitbook install
  ```

- For technical users _(ex: open source documentation)_, install the
  plugin to your **devDependencies** as follows:

  ```shell
  npm install --save-dev gitbook-plugin-folding-menu
  ```
