# vertical-layout

Stylus mixin for vertical layouts with both fluid and fixed elements. Employs absolute positioning, which, unlike calc-based grids, has solid Android support.

# Usage

```
vertical-layout: [top-stack-heights...] [fluid | fluid-gap] [bottom-stack-heights...]
```

## Restrictions

- There can only be one fluid element or fluid gap per container.
- All heights on either side of the gap have to be of the same unit
