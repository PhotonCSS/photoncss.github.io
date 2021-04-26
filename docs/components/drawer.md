# Drawer
Navigation drawers provide access to destinations in your app. [material.io](https://material.io/components/navigation-drawer)

## Importing
!!! info "Drawer components are an extension of the [`<List/>`](../list/) component"

```js hl_lines="2 6 7 8"
import React from "react";
import { Drawer } from "photoncss/react";

export default function Component() {
	return (
		<Drawer>
			...content
		</Drawer>
	);
}
```

## Props
| Name | Default | Possible Values | Type | Description |
| - | - | - | - | - |
| from | `left` | `left`, `right`, `top`, `bottom` | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | Sets the origin of the drawer to slide out from when opened. |
| swipe | `true` | Boolean value | [boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean) | Enables the drawer to be opened using a gesture on a touch display. |
!!! note
	Props other than those listed above such as `className` and `style` will be passed directly to the `<aside/>` element.

## Dynamic component
The snippet above **will not** render any visible content. To use Drawers to their full potential, incorperate the [`Photon.Drawer()`](../../public-methods/Drawer/) method.
