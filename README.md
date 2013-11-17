# Parser [![Build Status](https://travis-ci.org/chrisenytc/livi18n-parser.png?branch=master)](https://travis-ci.org/chrisenytc/livi18n-parser) [![Dependency Status](https://gemnasium.com/chrisenytc/livi18n-parser.png)](https://gemnasium.com/chrisenytc/livi18n-parser) [![NPM version](https://badge.fury.io/js/livi18n-parser.png)](http://badge.fury.io/js/livi18n-parser) [![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/chrisenytc/livi18n-parser/trend.png)](https://bitdeli.com/free "Bitdeli Badge")
> Parser API for internationalisation with Livi18n

## Instalation

Install from command line

`npm install livi18n-parser`

Install from package.json

```json
"dependencies": {
  "livi18n-parser": "~0.1.0"
}
```
Run this command to install

`npm install`


## Getting Started

```javascript
var parser = require('livi18n-parser');

//Translate API
var translate = parser.translate({test: ':name tested with successfully!'}, 'test', {name: 'translate'});

//Pluralize API
var pluralize = parser.pluralize({test: ':name have :&: iPhone||:name have :&: iPhones'}, 'test', {name: 'pluralize'}, 10);
```


## Documentation


#### .translate(data, key, options, defaultValue)

**Parameter**: `data`
**Type**: `JSON Object`
**Example**: `{test: ':name tested with successfully!'}`

**Parameter**: `key`
**Type**: `String`
**Example**: `test`

**Parameter**: `options`
**Type**: `JSON Object`
**Example**: `{name: 'translate'}`

**Parameter**: `defaultValue`
**Type**: `String`
**Example**: `Testing`

How to use init method

```javascript
parser.translate({test: ':name tested with successfully!'}, 'test', {name: 'translate'}); //translate tested with successfully!
```

#### .pluralize(data, key, options, nValue, defaultValue)

**Parameter**: `data`
**Type**: `JSON Object`
**Example**: `{test: ':name tested with successfully!'}`

**Parameter**: `key`
**Type**: `String`
**Example**: `test`

**Parameter**: `options`
**Type**: `JSON Object`
**Example**: `{name: 'translate'}`

**Parameter**: `nValue`
**Type**: `Integer`
**Example**: `10`

**Parameter**: `defaultValue`
**Type**: `String`
**Example**: `Testing`

How to use init method

```javascript
parser.pluralize({test: ':name have :&: iPhone||:name have :&: iPhones'}, 'test', {name: 'pluralize'}, 10); //pluralize have 10 iPhones
```

## Contributing

Please submit all issues and pull requests to the [chrisenytc/livi18n-parser](http://github.com/chrisenytc/livi18n-parser) repository!

## Support
If you have any problem or suggestion please open an issue [here](https://github.com/chrisenytc/livi18n-parser/issues).

## License
Copyright (c) 2013 Christopher EnyTC

Permission is hereby granted, free of charge, to any person
obtaining a copy of this software and associated documentation
files (the "Software"), to deal in the Software without
restriction, including without limitation the rights to use,
copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the
Software is furnished to do so, subject to the following
conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
OTHER DEALINGS IN THE SOFTWARE.

## Release History

 * 2013-11-17    v0.1.0   Initial release.

---
