# CardTitle
Cards contain content and actions about a single subject. [material.io](https://material.io/components/cards)

## Importing

```js hl_lines="2 7"
import React from "react";
import { Card, CardTitle } from "photoncss/react";

export default function Component() {
	return (
		<Card>
			<CardTitle>Title</CardTitle>
			...content
		</Card>
	);
}
```

## Props
| Name | Default | Possible Values | Type | Description |
| - | - | - | - | - |
| seperated | `true` | Boolean value  | [boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/BOOLEAN) | Determines if the title has an underline seperating it from the cards body content. |
| subtitle |  | String value | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | Sets subtitle of the card. |
!!! note
	Props other than those listed above such as `className` and `style` will be passed directly to the `<div/>` element.

***
**See also:**

* [Card](../card/)
