# Material-less

Developer friendly, CSS only, no JS, no classes, single file style sheet inspired by Material Design.

This style sheet changes the style of standard HTML5 elements to match the Material Design specification closely.
New elements are introduced to provide components with no HTML5 equivalent.

## Usage

Refer to the `materiallike.css` style sheet in this repository in the `<head>` element of your HTML document:

```
<link rel="stylesheet" href="style.css">
```

See `demo.html` for an example.

### Partial usage

The SASS source files are split into small modules, which can be compiled and used individually.
For correct font styling `html.scss` should be included.

### Dependencies

The style sheet automatically loads the Roboto and Material Icons fonts. There are no other runtime dependencies.

## Supported elements

### Standard HTML elements

The following standard HTML elements are explicitly styled:

* html  
* body
* table
* h1, h2, h3
* p
* button

#### New attributes

Some standard elements support additional attributes, which further specify their role or the nature of their content.

##### `<button>`

| Attribute | Values | Effect |
| --- | --- | --- |
| raised | none | raises button |
| colored | none | colors button in primary color |

### New elements:

The following new elements are defined:

##### `<i>`
Material Design icons as text characters.

##### `<card>`
"card" component. The content blocks defined in the Material Design specification are implemented by:
*`<h1>` for primary headings with optional `<hsub>` subtitles before or after the heading.
*`<p>` for supporting text
*`<button>` for action buttons.
