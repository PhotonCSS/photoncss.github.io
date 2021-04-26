# ThemeProvider
As of `v12`, themes are no longer LESS based or come precompiled. Now themes use CSS variables. Without using `<ThemeProvider/>` only basic styles will be rendered.

## Importing
```js hl_lines="2 6 7 8"
import React from "react";
import { ThemeProvider } from "photoncss/react";

export default function Component() {
	return (
		<ThemeProvider>
			...content goes here
		</ThemeProvider>
	);
}
```

## Props
| Name | Default | Possible Values | Type | Description |
| - | - | - | - | - |
| global | `false` | Boolean value | [boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean) | Tells the provider to override global CSS variables if true. If false, creates a scope and wraps content in a span element with the CSS variables. This is useful if you have a component subtree that you want to be a different theme than the root components. |
| theme | `default.light` | Any Photon theme | [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) \| [Theme](../../types/theme/) | Sets theme of the provider |

## Demo

### Global Theme Toggle
```js
import React, { useState } from "react";
import { render } from "react-dom";
import { ThemeProvider, Button } from "photoncss/react";
import "photoncss/dist/photon.css";

// Define array of themes that can be toggled through
const themes = [ "default.light", "default.dark" ];

export default function Root() {

	// Initialize theme state
	const [ themeId, setThemeId ] = useState(parseInt(localStorage.getItem("themeId") || "0"));

	// Define function to increment theme
	function nextTheme() {

		// Iterate to next theme in array or reset to first item
		let nextThemeId = themeId + 1;
		if(nextThemeId >= themes.length) nextThemeId = 0;

		// Save theme id and change state
		localStorage.setItem("themeId", nextThemeId);
		setThemeId(nextThemeId);

	}

	// Render component
	return (
		<ThemeProvider global theme={themes[themeId]}>

			<Button
				variant="raised"
				color="primary"
				onClick={nextTheme}>Switch to { themeId === 1 ? "light":"dark" } theme</Button>

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
