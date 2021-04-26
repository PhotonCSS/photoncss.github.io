# Column
The Material Design responsive layout grid adapts to screen size and orientation, ensuring consistency across layouts. [Material.io](https://material.io/design/layout/responsive-layout-grid)

## Importing

```js hl_lines="2 7 8 9"
import React from "react";
import { Row, Col } from "photoncss/react";

export default function Component() {
	return (
		<Row>
			<Col>
				...content
			</Col>
		</Row>
	);
}
```

## Props
| Name | Default | Possible Values | Type | Description |
| - | - | - | - | - |
| sm | `12` | Any number 1 - 12 | [number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number) | Sets the width out of 12 on small devices. |
| md | `12` | Any number 1 - 12 | [number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number) | Sets the width out of 12 on medium devices. |
| lg | `12` | Any number 1 - 12 | [number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number) | Sets the width out of 12 on large devices. |
| xl | `12` | Any number 1 - 12 | [number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number) | Sets the width out of 12 on extra-large devices. |
!!! note
	Props other than those listed above such as `className` and `style` will be passed directly to the `<div/>` element.

***
**See also:**

* [Container](../container/)
* [Row](../row/)
