# Icon
Material Icons are available in five styles and a range of downloadable sizes and densities. The icons are crafted based on the core design principles and metrics of Material design guideline. [material.io](https://material.io/design/iconography/system-icons)

## Importing

```js hl_lines="2 6"
import React from "react";
import { Icon } from "photoncss/react";

export default function Component() {
	return (
		<Icon>glyph</Icon>
	);
}
```
!!! note
	**Glyph's** are icons from the [Material Icon Font](https://fonts.google.com/icons), insert the icon name to display the icon.


## Props
| Name | Default | Possible Values | Type | Description |
| - | - | - | - | - |
| ink | `true` | Boolean value | [boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean) | Sets weather or not the icon should have a ripple/ink effect when interacted with. |
| variant | `normal` | `normal`, `outlined`, `round`, `sharp`, `two-tone` | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | Sets the variant of the icon. |
!!! note
	Props other than those listed above such as `className` and `style` will be passed directly to the `<i/>` element.

***
**See also:**

* [TextIcon](../texticon/)
