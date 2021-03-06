# highlightjs-line-numbers.js [![version](http://img.shields.io/badge/release-v1.0.0-brightgreen.svg?style=flat)](https://github.com/wcoder/highlightjs-line-numbers.js/archive/master.zip)

Highlight.js line numbers plugin.

## Usage

Download plugin and include file after highlight.js:
```html
<script src="highlight.min.js"></script>

<script src="dist/highlightjs-line-numbers.min.js"></script>
```

Adding styles:
```css
.hljs-line-numbers {
	text-align: right;
	border-right: 1px solid #ccc;
	color: #999;
	-webkit-touch-callout: none;
	-webkit-user-select: none;
	-khtml-user-select: none;
	-moz-user-select: none;
	-ms-user-select: none;
	user-select: none;
}
```

Initialize plugin after highlight.js:
```js
hljs.initHighlightingOnLoad();

hljs.initLineNumbersOnLoad();
```

Here’s an equivalent way to calling `initLineNumbersOnLoad` using jQuery:
```js
$(document).ready(function() {
	$('code.hljs').each(function(i, block) {
		hljs.lineNumbersBlock(block);
	});
});
```

&copy; 2015 Yauheni Pakala | MIT License
