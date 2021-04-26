# Photon.Snackar()
Interact with [`<Snackar/>`](../../components/snackbar/) components in the DOM.

## Importing
```js
import Photon from "photoncss";
```
!!! warning "Use the default export"

## Usage
```js
Photon.Snackbar(<Snackbar/>, options);
```
**returns** new [Snackbar](./#Class)

### Arguments
| Argument | Type | Description |
| - | - | - |
| snackbar | JSX | Snackbar element. |
| options | [Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object) | Snackbar options. |
| options.id? | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) | Snackbar ID. |
| options.duration? | [number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number) \| [null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Null) | Time in milliseconds to show snackbar for, use null to show forever. |

## Class

### Properties
`.isOpen` : [boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)
> Gets if the drawer is open.

`.snackbar` : [jQuery](https://api.jquery.com/jQuery/)
> Get the drawer element on the DOM.

`.options` : [Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)
> Get the options the snackbar was shown with.

### Methods
`.close()` : [this](./)
> Closes the drawer.

`.open()` : [this](./)
> Closes the drawer.

# Example
```js
import React, { Fragment } from "react";
import Photon from "photoncss";
import { Button, Snackbar } from "photoncss/react";

export function MySnackbar() {
	return (
		<Snackbar>
			<p>Hi, im a drawer</p>
		</Snackbar>
	);
}

export default function Component() {
    return (
        <Fragment>

			<Button
			  color="primary"
			  variant="raised"
			  onClick={ () => Photon.Snackbar(<MySnackbar/>) }>Show snackbar</Button>

        </Fragment>
    );
}
```
