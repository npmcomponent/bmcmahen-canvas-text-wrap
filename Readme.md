*This repository is a mirror of the [component](http://component.io) module [bmcmahen/canvas-text-wrap](http://github.com/bmcmahen/canvas-text-wrap). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/bmcmahen-canvas-text-wrap`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# canvas-text-wrap

text wrapping for canvas

## Installation

	$ component install bmcmahen/canvas-text-wrap

## API

### wrap(context, string, x, y, maxWidth, lineHeight)

The wrap function returns an array of text lines, each consisting of an object with `text`, `x`, and `y` position. This can be more efficient when animating so that you don't need to recalculate the text-wrap during each discrete step.


## Example

	var wrap = require('bmcmahen-canvas-text-wrap');
	var txt = wrap(ctx, 'this is a long string that should be truncated, i think', 0, 0, 55, 15);
	for (var i = 0; i < txt.length; i++){
		var item = txt[i];
		ctx.fillText(item.text, item.x, item.y);
	}

## License

	MIT
