# modal

A simple modal UI component.

Rewrite of [segmentio/modal](https://github.com/segmentio/modal) for
npm+browserify support.

## Example

``` javascript
var Modal = require('modal');

var modal = new Modal(el);
modal.show();
```

## Installation

``` bash
$ npm install KenanY/modal
```

## API

``` html
<div class="Modal">
  { Your element gets injected here. }
</div>
```

A [KenanY/overlay](https://github.com/KenanY/overlay) element (with an
`.Overlay` class) is used to create the mask above the screen, so if you've
already themed it you've got no more work to do.

``` javascript
var Modal = require('modal');
```

### var modal = new Modal(el)

Create a new `Modal` instance with the given `el`.

### modal.show(fn)

Show the modal, emitting `show`, optionally calling `fn`.

### modal.hide(fn)

Hide the modal, emitting `hide`, optionally calling `fn`.

### modal.closeable()

Make the modal closeable.

Alias: `modal.closable()`

### modal.overlay()

Shows an overlay with the modal.

### modal.effect(name)

See the effect `name`. Comes bundled with `toggle`, `slide-in-bottom`,
`sticky-up`, and `fade-and-scale`.

### modal.addClass(name)

Add a class `name` to the `.Modal`.

### modal.removeClass(name)

Remove a class `name` from the `.Modal`.