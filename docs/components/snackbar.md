# Snackbar
Snackbars provide brief messages about app processes at the bottom of the screen. [material.io](https://material.io/components/snackbars)

## Importing

```js hl_lines="2 6 7 8 9"
import React from "react";
import { Button, Snackbar } from "photoncss/react";

export default function Component() {
	return (
		<Snackbar>
			<p>I am a snackbar!</p>
			<Button variant="flat" color="secondary">action</Button>
		</Snackbar>
	);
}
```
The snippet above displays a static snackbar. To use them to send the user notifications, you must use the [`Photon.Snackbar()`](../../public-methods/Snackbar/) method.
