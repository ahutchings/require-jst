# require-jst

A RequireJS/AMD loader plugin for loading compiled [Underscore](http://underscorejs.org)
templates.

## Usage

This plugin depends on the [text plugin](https://github.com/requirejs/text) for
loading templates dynamically. The same XHR restrictions apply as for the text
plugin.

For production use, the **text** and **jst** plugins can be stubbed and
template functions can be precompiled with the [RequireJS Optimizer](http://requirejs.org/docs/optimization.html).

You can load a compiled Underscore template like so:

```javascript
require(['jst!templates/module.jst'],
	function (template) {
		// the template variable here is a template function
	}
);
```
