# Container
Containers are used to give the appropriate amount of padding on the left and right sides of your main content. These are used to prevent your content from being out of proportion on high resolution displays.

## Importing

```js hl_lines="2 6 7 8"
import React from "react";
import { Container } from "photoncss/react";

export default function Component() {
	return (
		<Container>
			...content
		</Container>
	);
}
```

*** 
**See also:**

* [Column](../column/)
* [Row](../row/)
