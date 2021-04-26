# InputField
Text fields let users enter and edit text. [material.io](https://material.io/components/text-fields)

## Importing

```js hl_lines="2 6"
import React from "react";
import { InputField } from "photoncss/react";

export default function Component() {
	return (
		<InputField/>
	);
}
```

## Props
| Name | Default | Possible Values | Type | Description |
| - | - | - | - | - |
| color | `none` | `none`, `primary`, `secondary` | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | Sets the color of the field. |
| variant | `normal` | `normal`, `outlined`, `filled` | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | Sets the variant of the field. |
| prefix |  | String value | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | Sets the prefix of the field. |
| suffix |  | String value | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | Sets the suffix of the field. |
| subtitle |  | String value | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | Sets the subtitle of the field. |
| dropdown |  | Array of String values | [array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)<[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)> | Makes the field a dropdown and sets the possible options. |

!!! note
	Props other than those listed above such as `className` and `style` will be passed directly to the wrapper element while input props will go to the `<input/>` element.
