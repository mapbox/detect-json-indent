[![Build Status](https://travis-ci.org/tmcw/detect-json-indent.png)](https://travis-ci.org/tmcw/detect-json-indent)

## detect JSON indent

```js
detect(JSON.stringify(data, null, 4)) // '    '
detect(JSON.stringify(data, null, '\t')) // '\t'
detect(JSON.stringify(data, null, 2)) // '  '
detect(JSON.stringify(data)) // null
```

### api

```js
var detect = require('detect-json-indent');
var indentString = detect(jsonString);
```
