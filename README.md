# v-layout

Stylus mixin for vertical layouts with any number of fixed-height elements and an optional fluid element or gap. Employs absolute positioning, which, unlike calc-based grids, has been supported by Android for a while now.

## Installation

```
npm i v-layout
```

In your stylesheet:

```
@import '~v-layout'
```

## Usage

```
.container
  position: relative
  v-layout: [full-width] [top-stack-heights...] [fluid | fluid-gap] [bottom-stack-heights...]
```

[Check out the examples.](http://bopjesvla.github.io/v-layout)

## Restrictions

- There can only be one fluid element or fluid gap per container.
- All heights on either side of the gap have to be of the same unit
- The container must be positioned (`position: relative` usually has no other side effects)
