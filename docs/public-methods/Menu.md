# Photon.Menu()
Interact with [`<Menu/>`](../../components/menu/) components in the DOM.

## Importing
```js
import Photon from "photoncss";
```
!!! warning "Use the default export"

## Usage
```js
Photon.Menu(menu_element);
```
**returns** new [Menu](./#Class)

### Arguments
| Argument | Type | Description |
| - | - | - |
| menu_element | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) \| [jQuery](https://api.jquery.com/jQuery/) \| [Element](https://developer.mozilla.org/en-US/docs/Web/API/Element) | Any of the allowed types that resolves to an element on the DOM. |

## Class

### Properties
`.isOpen` : [boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)
> Gets if the menu is open.

`.target` : [jQuery](https://api.jquery.com/jQuery/)
> Get the menu element on the DOM.

### Methods
`.anchor(positionX: number, positionY: number)` : [this](./)

`.anchor(anchorToElement: string | jQuery | Element)` : [this](./)
> Sets the menu position.

`.close()` : [this](./)
> Closes the menu.

`.open()` : [this](./)
> Closes the menu.

# Example
```js
import React, { Fragment } from "react";
import Photon from "photoncss";
import { Button, Menu } from "photoncss/react";

export function MyMenu() {
	return (
		<Menu id="my-menu">
			Hi, im a menu
		</Menu>
	);
}

export default function Component() {
    return (
        <Fragment>

			<MyMenu/>

			<Button
			  color="primary"
			  variant="raised"
			  onClick={ () => Photon.Menu("#my-menu").open() }>Show menu</Button>

        </Fragment>
    );
}
```
