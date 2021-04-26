# ListItem
Lists are continuous, vertical indexes of text or images. [material.io](https://material.io/components/lists)

## Importing
```js hl_lines="2 6"
import React from "react";
import { ListItem } from "photoncss/react";

export default function Component() {
	return (
		<ListItem>content</ListItem>
	);
}
```

## Props
| Name | Default | Possible Values | Type | Description |
| - | - | - | - | - |
| icon | `null` | TextIcon | [TextIcon](../texticon/) | Sets the icon in the front of the content. |
| iconEnd | `null` | TextIcon | [TextIcon](../texticon/) | Sets the icon in the end of the content. |
| round | `false` | Boolean value | [boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean) | Sets if the list item should have rounded corners. |
| waves | `true` | Boolean value | [boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean) | Sets if the list item should utilize waves/ripples when interacted with.
!!! note
	Props other than those listed above such as `className` and `style` will be passed directly to the `<;i/>` element.

***
**See also:**

* [List](../list/)
