# Menu
Menus display a list of choices on temporary surfaces. [material.io](https://material.io/components/menus)

## Importing
!!! info "Menu components are an extension of the [`<List/>`](../list/) component"

```js hl_lines="2 6 7 8"
import React from "react";
import { Menu } from "photoncss/react";

export default function Component() {
	return (
		<Menu>
			...content
		</Menu>
	);
}
```

## Dynamic component
The snippet above **will not** render any visible content. To use Menus to their full potential, incorperate the [`Photon.Menu()`](../../public-methods/Menu/) method.
