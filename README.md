# v-layout

Stylus mixin for vertical layouts with both fluid and fixed-height elements. Employs absolute positioning, which, unlike calc-based grids, has been supported by Android for a while now.

## Usage

```
.container
  position: relative
  v-layout: [full-width] [top-stack-heights...] [fluid | fluid-gap] [bottom-stack-heights...]
```

[Check out the examples.](http://bopjesvla.github.io/stylus-vertical-layout)

## Restrictions

- There can only be one fluid element or fluid gap per container.
- All heights on either side of the gap have to be of the same unit
- The container must be positioned (`position: relative` usually has no other side effects)
