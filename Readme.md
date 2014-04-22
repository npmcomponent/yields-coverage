*This repository is a mirror of the [component](http://component.io) module [yields/coverage](http://github.com/yields/coverage). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/yields-coverage`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# Coverage

  code coverage in your browser

## Installation

```bash
$ component install yields/coverage
```

## Example

clone and run `$ make example`.

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset='utf8'>
    <title>yields-lru-cache</title>
    <link rel='stylesheet' href='../build/build.css'>
    <script src='../build/build.js'></script>
    <script>require('mocha')</script>
    <script>mocha.setup({ ui: 'bdd' })</script>
  </head>
  <body>
    <div id='coverage'></div>
    <div id='mocha' style='display: none;'></div>
    <script>cov = require('coverage')('yields-lru-cache');</script>
    <script src='test.js'></script>
    <script>mocha.run(cov.render.bind(cov))</script>
  </body>
</html>
```

## API

### Coverage()

  Initialize `Coverage` with `name`. (component name)

#### #render()

  Render to `#coverage`

## License

(MIT)
