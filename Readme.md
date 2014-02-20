*This repository is a mirror of the [component](http://component.io) module [juliangruber/get-user-media](http://github.com/juliangruber/get-user-media). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/juliangruber-get-user-media`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# get-user-media

  Cross browser navigator.getUserMedia with a node api.

## Example

```js
var getUserMedia = require('get-user-media');

getUserMedia({ audio: true }, function(err, stream) {
  if (err) throw err;

  // do something with the stream
});
```

## API

### getUserMedia(constraints, fn)

  Request user media based on given `constraints`, which currently can be
  
```js
{
  audio: true,
  video: true
}
```
  
  Call `fn` with the potential `Error` and the resulting input stream.

## Installation

  Install with [npm](https://npmjs.org):
  
    $ npm install get-user-media
  
  Install with [component(1)](http://component.io):
  
    $ component install juliangruber/get-user-media

## License

  MIT
