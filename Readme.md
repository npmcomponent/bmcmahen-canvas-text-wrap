
# canvas-text-wrap

	text wrapping for canvas

## Installation

		$ component install bmcmahen/canvas-text-wrap

## API

	var wrap = require('canvas-text-wrap');
	var txt = wrap(ctx, 'this is a long string that should be truncated, i think', 0, 0, 55, 15);
	for (var i = 0; i < txt.length; i++){
		var item = txt[i];
		ctx.fillText(item.text, item.x, item.y);
	}

## License

	MIT