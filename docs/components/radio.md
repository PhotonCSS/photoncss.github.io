# Radio
Radio buttons allow users to select one option from a set. [material.io](https://material.io/components/radio-buttons)

## Importing

```js hl_lines="2 6"
import React from "react";
import { Radio } from "photoncss/react";

export default function Component() {
	return (
		<Radio>text</Radio>
	);
}
```

## Props
| Name | Default | Possible Values | Type | Description |
| - | - | - | - | - |
| color | `none` | `none`, `primary`, `secondary` | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | Sets the color of the button. |
| labelPosition | `after` | `before`, `after` | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | Sets which comes first, the label or the radio button. |
| waves | `true` | Boolean value | [boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean) | Sets weather or not the radio button should have a ripple/waves effect when interacted with. |


!!! note
	Props other than those listed above such as `className` and `style` will be passed directly to the `<input/>` element.
