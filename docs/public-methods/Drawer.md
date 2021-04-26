# Photon.Drawer()
Interact with [`<Drawer/>`](../../components/drawer/) components in the DOM.

## Importing
```js
import Photon from "photoncss";
```
!!! warning "Use the default export"

## Usage
```js
Photon.Drawer(drawer_element);
```
**returns** new [Drawer](./#Class)

### Arguments
| Argument | Type | Description |
| - | - | - |
| drawer_element | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) \| [jQuery](https://api.jquery.com/jQuery/) \| [Element](https://developer.mozilla.org/en-US/docs/Web/API/Element) | Any of the allowed types that resolves to an element on the DOM. |

## Class

### Properties
`.isOpen` : [boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)
> Gets if the drawer is open.

`.target` : [jQuery](https://api.jquery.com/jQuery/)
> Get the drawer element on the DOM.

### Methods
`.close()` : [this](./)
> Closes the drawer.

`.open()` : [this](./)
> Closes the drawer.

# Example
```js
import React, { Fragment } from "react";
import Photon from "photoncss";
import { Button, Drawer } from "photoncss/react";

export function MyDrawer() {
	return (
		<Drawer id="my-drawer">
			Hi, im a drawer
		</Drawer>
	);
}

export default function Component() {
    return (
        <Fragment>

			<MyDrawer/>

			<Button
			  color="primary"
			  variant="raised"
			  onClick={ () => Photon.Drawer("#my-drawer").open() }>Show drawer</Button>

        </Fragment>
    );
}
```
