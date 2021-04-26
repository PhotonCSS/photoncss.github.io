# Card
Cards contain content and actions about a single subject. [material.io](https://material.io/components/cards)

## Importing

```js hl_lines="2 6 7 8"
import React from "react";
import { Card } from "photoncss/react";

export default function Component() {
	return (
		<Card>
			...content
		</Card>
	);
}
```

## Props
| Name | Default | Possible Values | Type | Description |
| - | - | - | - | - |
| display | `block` | `block`, `inline` | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | Sets the display property of the button. |
| variant | `raised` | `outlined`, `raised` | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | Sets the variant of the card. |
!!! note
	Props other than those listed above such as `className` and `style` will be passed directly to the `<div/>` element.

***
**See also:**

* [CardActions](../cardactions/)
* [CardBody](../cardbody/)
* [CardImage](../cardimage/)
* [CardOverline](../cardoverline/)
* [CardSubheader](../cardsubheader/)
* [CardSubtitle](../cardsubtitle/)
* [CardTitle](../cardtitle/)
