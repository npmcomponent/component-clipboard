*This repository is a mirror of the [component](http://component.io) module [component/clipboard](http://github.com/component/clipboard). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/component-clipboard`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# Clipboard

  Clipboard library.

## Installation

```
$ component install component/clipboard
```

## Example

```js
var Clipboard = require('clipboard');
var clip = new Clipboard(window);

clip.on('paste', function(e){
  e.items.forEach(function(item){
    console.log(item);
  });
});

clip.on('cut', function(){
  console.log('cut');
});

clip.on('copy', function(e){
  console.log('copy');
});
```

## API

### Clipboard#bind()

  Bind event handlers. This is done for you in the constructor.

### Clipboard#unbind()

  Unbind event handlers.

## Links

  - w3c [clipboard apis](http://www.w3.org/TR/clipboard-apis/)

## License

 MIT
