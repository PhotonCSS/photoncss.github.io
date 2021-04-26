# Getting Started Guide
Install Photon and its dependencies.
```bash
npm install --save-dev photoncss jquery react react-dom
```

## Set up the main file
```js hl_lines="3 4 9 11"
import React from "react";
import { render } from "react-dom";
import { ThemeProvider } from "photoncss/react"; 	// Import Photon in to the project
import "photoncss/dist/photon.css"; 				// Import the Photon stylesheet

// Create the root element
export function Root() {
	return (
		<ThemeProvider global>
			<p>PhotonCSS Demo</p>
		</ThemeProvider>
	);
}

// Wait for the DOM to load before rendering
document.addEventListener("DOMContentLoaded", function() {

	// Append a container to the DOM to render content into
	const root = document.createElement("DIV");
	root.id = "root";
	document.body.append(root);

	// Render root component into react-root container
	render(<Root/>, document.getElementById("root"));

});
```

## Importing components
All components are imported from the module `photoncss/react`.

```js hl_lines="1 6"
import { Button } from "photoncss/react"

export function Root() {
	return (
		<ThemeProvider global>
			<Button variant="raised" color="primary">Hello World</Button>
		</ThemeProvider>
	);
}
```

## Using custom themes
For custom themes, you need the [`<ThemeProvider/>`](../components/themeprovider) component.
