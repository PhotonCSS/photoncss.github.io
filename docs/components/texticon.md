# TextIcon
Material Icons are available in five styles and a range of downloadable sizes and densities. The icons are crafted based on the core design principles and metrics of Material design guideline. [material.io](https://material.io/design/iconography/system-icons)

## Importing

```js hl_lines="2 6 7 8"
import React from "react";
import { TextIcon } from "photoncss/react";

export default function Component() {
	return (
		<p>
			This is a paragraph that contains a <TextIcon>menu</TextIcon> icon!
		</p>
	);
}
```
!!! note
	**Glyph's** are icons from the [Material Icon Font](https://fonts.google.com/icons), insert the icon name to display the icon.


## Props
| Name | Default | Possible Values | Type | Description |
| - | - | - | - | - |
| variant | `normal` | `normal`, `outlined`, `round`, `sharp`, `two-tone` | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | Sets the variant of the icon. |
!!! note
	Props other than those listed above such as `className` and `style` will be passed directly to the `<i/>` element.

***
**See also:**

* [Icon](../icon/)
