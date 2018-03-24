# Material-less

Developer friendly, CSS only, no JS, no classes, single file style sheet inspired by Material Design.

This style sheet changes the style of standard HTML5 elements to look similar to Material Design components.
New elements are introduced to provide components with no HTML5 equivalents.

### Dependencies

The only dependency of the style sheet is the Material Icons font, if `<i>` elements are used.
The corresponding `icons.woff` file can be found in this repository.
It should be hosted in the same directory as style sheet.
Alternatively, it may be loaded from Google Web Fonts, by adding the following line to your page header:
```
<link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">
```

## Demo

Have a look at [demo.html](http://htmlpreview.github.io/?https://github.com/infobaleen/material-less/blob/master/demo.html).

## Usage

Refer to the `material-less.css` style sheet in this repository in the `<head>` element of your HTML document.

```
<link rel="stylesheet" href="material-less.css">
```

Alternatively you can use `@import "<path>/material-less.scss";` in your own SASS files.
Individual components can be selectively included using the respective SASS (e.g. `@import "<path>/button.scss"`) file.

### Customization

The color scheme can be customized via CSS variables. Use the `:root` selector to change the color scheme for the whole document:
```
 :root {
        --colorPrimary: red;
        --colorPrimaryLight: tomato;
        --colorPrimaryDark: darkred;
    }
```

## Supported elements

### Supported HTML elements without additional attributes

* `<a>`
* `<body>`
* `<details>`
* `<h1>`, `<h2>`, `<h3>`
* `<html>`
* `<hr>`
* `<input>` (see `<button>` for `<input type="button">`)
* `<p>`
* `<select>`
* `<table>`

### Supported HTML elements with additional attributes

#### `<button>`

| Attribute | Values | Effect |
| --- | --- | --- |
| raised | none | raises button |
| colored | none | colors button in primary color |

#### `<nav>`

| Attribute | Values | Effect |
| --- | --- | --- |
| sticky | none | nav sticks to top |

### New elements:

The following new elements are defined:

#### `<i>`
Material Design icons. Example: `<i>check_circle</i>`.

#### `<hsub>`
Subtitles. Use before or after `<h1>`, `<h2>`, or `<h3>`.

#### `<card>`
Card component. The content blocks defined in the Material Design specification are implemented by:
* `<h1>` for primary headings with optional `<hsub>` subtitles before or after the heading.
* `<p>` for supporting text
* `<button>` for action buttons.
