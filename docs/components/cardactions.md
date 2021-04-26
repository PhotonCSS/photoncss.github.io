# CardActions
Cards contain content and actions about a single subject. [material.io](https://material.io/components/cards)

## Importing

```js hl_lines="2 8 11"
import React from "react";
import { Button, Card, CardActions } from "photoncss/react";

export default function Component() {
	return (
		<Card>
			...content
			<CardActions>
				<Button variant="flat" color="primary">Action 1<Button>
				<Button variant="flat" color="primary">Action 2<Button>
			</CardActions>
		</Card>
	);
}
```

## Props
| Name | Default | Possible Values | Type | Description |
| - | - | - | - | - |
| direction | `left` | `left`, `right` | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | Defines where the action buttons appear. |
| seperated | `true` | Boolean value  | [boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/BOOLEAN) | Determines if the title has an underline seperating it from the cards body content. |
!!! note
	Props other than those listed above such as `className` and `style` will be passed directly to the `<div/>` element.

***
**See also:**

* [Card](../card/)
