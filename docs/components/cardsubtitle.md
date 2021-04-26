# CardSubtitle
Cards contain content and actions about a single subject. [material.io](https://material.io/components/cards)

!!! warning
	Not to be confused with the `subtitle` prop on the [`<CardTitle/>`](../cardtitle/) component or the [`<CardSubheader/>`](../cardsubheader/) component.

## Importing

```js hl_lines="2 8"
import React from "react";
import { Card, CardSubtitle } from "photoncss/react";

export default function Component() {
	return (
		<Card>
			...content
			<CardSubtitle>Subheader</CardSubtitle>
			...content
		</Card>
	);
}
```

***
**See also:**

* [Card](../card/)
