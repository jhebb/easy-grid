easy-grid
=========

A semantic Sass grid system using margins.

Allows grid items with background colors and padding for immediate content instead of needing a wrapper on each grid item.

By: [Justin Hebb](http://jukah.com)

Based on ideas from:
- [Zen Grids](https://github.com/JohnAlbin/zen-grids)
- [Semantic Grid System](https://github.com/twigkit/semantic.gs/)
- [Fluid-Grid](https://github.com/akikoo/Fluid-Grid)

##Demo
http://jhebb.github.io/easy-grid/

##Known Issues
- gutter needs to be percentage based
- grid containers that don't fit full-width don't clear grid containers below them. May need "clear: both" on grid containers.
- margin-bottom is inconsistent since it's percentage-based for grid-items and fixed for grid-container. Need a best of both. Maybe add an option to mixin for margin-bottom


##Todo
- [ ] test further
- [ ] add bottom margin to grid-container?
- [ ] move margin-bottom to grid-container instead of removing from last-child?
- [ ] how to reset $columns on the next grid-container if it's been redefined
- [ ] change names of nested boxes/classes to be clearer
- [ ] try switching to margin-left and always hiding first-child. May eliminate need for having to remove margin on containers with more than one row of columns