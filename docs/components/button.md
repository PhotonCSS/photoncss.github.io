# Button
Buttons allow users to take actions, and make choices, with a single tap. [material.io](https://material.io/components/buttons)

## Importing

```js hl_lines="2 6"
import React from "react";
import { Button } from "photoncss/react";

export default function Component() {
	return (
		<Button>text</Button>
	);
}
```

## Props
| Name | Default | Possible Values | Type | Description |
| - | - | - | - | - |
| color | `none` | `none`, `primary`, `secondary` | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | Sets the color of the button. |
| display | `inline` | `block`, `inline` | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | Sets the display property of the button. |
| size | `normal` | `dense`, `normal`, `large` | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | Sets the size of the button. |
| variant | `contained` | `contained`, `flat`, `outlined`, `raised` | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | Sets the variant of the button. |
| waves | `true` | Boolean value | [boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean) | Sets weather or not the button should have a ripple/waves effect when interacted with. |
!!! note
	Props other than those listed above such as `className` and `style` will be passed directly to the `<button/>` element.
