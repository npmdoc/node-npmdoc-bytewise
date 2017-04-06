# api documentation for  [bytewise (v1.1.0)](https://github.com/deanlandolt/bytewise)  [![npm package](https://img.shields.io/npm/v/npmdoc-bytewise.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-bytewise) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-bytewise.svg)](https://travis-ci.org/npmdoc/node-npmdoc-bytewise)
#### Binary serialization which sorts bytewise for arbirarily complex data structures

[![NPM](https://nodei.co/npm/bytewise.png?downloads=true)](https://www.npmjs.com/package/bytewise)

[![apidoc](https://npmdoc.github.io/node-npmdoc-bytewise/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-bytewise_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-bytewise/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-bytewise/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-bytewise/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Dean Landolt",
        "email": "dean@deanlandolt.com"
    },
    "bugs": {
        "url": "https://github.com/deanlandolt/bytewise/issues"
    },
    "dependencies": {
        "bytewise-core": "^1.2.2",
        "typewise": "^1.0.3"
    },
    "description": "Binary serialization which sorts bytewise for arbirarily complex data structures",
    "devDependencies": {
        "faucet": "0.0.1",
        "tape": "^1.0.0"
    },
    "directories": {},
    "dist": {
        "shasum": "1d13cbff717ae7158094aa881b35d081b387253e",
        "tarball": "https://registry.npmjs.org/bytewise/-/bytewise-1.1.0.tgz"
    },
    "gitHead": "eb8fbdb2ff1aeff3f7486a66ec84c8fb3db46e5b",
    "homepage": "https://github.com/deanlandolt/bytewise",
    "keywords": [
        "binary",
        "sort",
        "collation",
        "serialization",
        "leveldb",
        "indexeddb"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "deanlandolt",
            "email": "dean@deanlandolt.com"
        }
    ],
    "name": "bytewise",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/deanlandolt/bytewise.git"
    },
    "scripts": {
        "test": "tape test | faucet"
    },
    "version": "1.1.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module bytewise](#apidoc.module.bytewise)
1.  boolean <span class="apidocSignatureSpan">bytewise.</span>buffer
1.  [function <span class="apidocSignatureSpan">bytewise.</span>compare (a, b)](#apidoc.element.bytewise.compare)
1.  [function <span class="apidocSignatureSpan">bytewise.</span>decode (buffer, options)](#apidoc.element.bytewise.decode)
1.  [function <span class="apidocSignatureSpan">bytewise.</span>encode (source, options)](#apidoc.element.bytewise.encode)
1.  [function <span class="apidocSignatureSpan">bytewise.</span>equal (a, b)](#apidoc.element.bytewise.equal)
1.  [function <span class="apidocSignatureSpan">bytewise.</span>getType (byte)](#apidoc.element.bytewise.getType)
1.  [function <span class="apidocSignatureSpan">bytewise.</span>postDecode (decoded, options)](#apidoc.element.bytewise.postDecode)
1.  [function <span class="apidocSignatureSpan">bytewise.</span>postEncode (encoded, options)](#apidoc.element.bytewise.postEncode)
1.  object <span class="apidocSignatureSpan">bytewise.</span>bound
1.  object <span class="apidocSignatureSpan">bytewise.</span>bound.sort
1.  object <span class="apidocSignatureSpan">bytewise.</span>hex
1.  object <span class="apidocSignatureSpan">bytewise.</span>sorts
1.  object <span class="apidocSignatureSpan">bytewise.</span>stringCodec
1.  string <span class="apidocSignatureSpan">bytewise.</span>type

#### [module bytewise.bound](#apidoc.module.bytewise.bound)
1.  [function <span class="apidocSignatureSpan">bytewise.bound.</span>compare (a, b)](#apidoc.element.bytewise.bound.compare)
1.  [function <span class="apidocSignatureSpan">bytewise.bound.</span>encode (data, base)](#apidoc.element.bytewise.bound.encode)
1.  [function <span class="apidocSignatureSpan">bytewise.bound.</span>getBoundary (source)](#apidoc.element.bytewise.bound.getBoundary)
1.  object <span class="apidocSignatureSpan">bytewise.bound.</span>sort

#### [module bytewise.bound.sort](#apidoc.module.bytewise.bound.sort)
1.  [function <span class="apidocSignatureSpan">bytewise.bound.sort.</span>compare (a, b)](#apidoc.element.bytewise.bound.sort.compare)
1.  [function <span class="apidocSignatureSpan">bytewise.bound.sort.</span>equal (a, b)](#apidoc.element.bytewise.bound.sort.equal)
1.  [function <span class="apidocSignatureSpan">bytewise.bound.sort.</span>invalid (a, b)](#apidoc.element.bytewise.bound.sort.invalid)
1.  object <span class="apidocSignatureSpan">bytewise.bound.sort.</span>bound
1.  object <span class="apidocSignatureSpan">bytewise.bound.sort.</span>order
1.  object <span class="apidocSignatureSpan">bytewise.bound.sort.</span>sorts

#### [module bytewise.hex](#apidoc.module.bytewise.hex)
1.  boolean <span class="apidocSignatureSpan">bytewise.hex.</span>buffer
1.  [function <span class="apidocSignatureSpan">bytewise.hex.</span>decode (buffer)](#apidoc.element.bytewise.hex.decode)
1.  [function <span class="apidocSignatureSpan">bytewise.hex.</span>encode (source)](#apidoc.element.bytewise.hex.encode)
1.  string <span class="apidocSignatureSpan">bytewise.hex.</span>type

#### [module bytewise.stringCodec](#apidoc.module.bytewise.stringCodec)
1.  [function <span class="apidocSignatureSpan">bytewise.stringCodec.</span>decode (buffer)](#apidoc.element.bytewise.stringCodec.decode)
1.  [function <span class="apidocSignatureSpan">bytewise.stringCodec.</span>encode (source)](#apidoc.element.bytewise.stringCodec.encode)



# <a name="apidoc.module.bytewise"></a>[module bytewise](#apidoc.module.bytewise)

#### <a name="apidoc.element.bytewise.compare"></a>[function <span class="apidocSignatureSpan">bytewise.</span>compare (a, b)](#apidoc.element.bytewise.compare)
- description and source-code
```javascript
compare = function (a, b) {
  //
  // test for invalid values
  //
  if (base.invalid(a, b))
    return NaN

  //
  // short circuit for identical objects
  //
  if (a === b)
    return 0

  //
  // short circuit for base bound types
  //
  var result = base.bound.compare(a, b)
  if (result !== undefined)
    return result

  //
  // cache typeof and valueOf for both values
  //
  var aTypeOf = typeof a
  var bTypeOf = typeof b
  var aValueOf = _valueOf(a)
  var bValueOf = _valueOf(b)

  //
  // loop over type tags and attempt compare
  //
  var order = base.order
  var sorts = base.sorts
  var sort
  for (var i = 0, length = order.length; i < length; ++i) {
    sort = sorts[order[i]]

    //
    // if first arg is a member of this sort we have an answer
    //
    if (sort.is(a, aTypeOf))
      //
      // if b is the same as a then defer to sort's comparator, else a comes first
      //
      return sort.is(b, bTypeOf) ? sort.compare(aValueOf, bValueOf) : -1

    //
    // if b is this type but not a then b comes first
    //
    if (sort.is(b, bTypeOf))
      return 1
  }

  //
  // values are incomparable as they didn't match against any registered types
  //
  return NaN
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bytewise.decode"></a>[function <span class="apidocSignatureSpan">bytewise.</span>decode (buffer, options)](#apidoc.element.bytewise.decode)
- description and source-code
```javascript
decode = function (buffer, options) {
  // attempt to decode string input using configurable codec
  if (typeof buffer === 'string') {
    buffer = bytewise.stringCodec.encode(buffer)
  }

  assert(!buffer || !buffer.undecodable, 'Encoded value not decodable')

  var byte = buffer[0]
  var type = bytewise.getType(byte)
  assert(type, 'Invalid encoding: ' + buffer)

  // if type provides a decoder it is passed the base type system as second arg
  var codec = type.codec
  if (codec) {
    var decoded = codec.decode(buffer.slice(1), bytewise)

    if (options && options.nested && codec.unescape)
      decoded = codec.unescape(decoded)

    return postDecode(decoded, options)
  }

  // nullary types without a codec must provide a value for their decoded form
  assert('value' in type, 'Unsupported encoding: ' + buffer)
  return postDecode(type.value, options)
}
```
- example usage
```shell
...
var core = require('./binary')

exports.encode = function (source) {
  return core.encode(source).toString('hex')
}

exports.decode = function (buffer) {
  return core.decode(buffer.toString('hex'))
}

exports.buffer = false;
exports.type = 'bytewise-hex';
...
```

#### <a name="apidoc.element.bytewise.encode"></a>[function <span class="apidocSignatureSpan">bytewise.</span>encode (source, options)](#apidoc.element.bytewise.encode)
- description and source-code
```javascript
encode = function (source, options) {

  // check for invalid/incomparable values
  assert(!base.invalid(source), 'Invalid value')

  // encode bound types (ranges)
  var boundary = base.bound.getBoundary(source)
  if (boundary)
    return boundary.encode(source, bytewise)

  // encode standard value-typed sorts
  var order = base.order
  var sort
  for (var i = 0, length = order.length; i < length; ++i) {
    sort = sorts[order[i]]

    if (sort.is(source)) {

      // loop over any subsorts defined on sort
      // TODO: clean up
      var subsorts = sort.sorts ||  { '': sort }
      for (key in subsorts) {
        var subsort = subsorts[key]
        if (subsort.is(source))
          return serialize(subsort, source, options)
      }

      // source is an unsupported subsort
      assert(false, 'Unsupported sort value')
    }
  }

  // no type descriptor found
  assert(false, 'Unknown value')
}
```
- example usage
```shell
...


// TODO: encoding class hierarchy

var core = require('./binary')

exports.encode = function (source) {
  return core.encode(source).toString('hex')
}

exports.decode = function (buffer) {
  return core.decode(buffer.toString('hex'))
}

exports.buffer = false;
...
```

#### <a name="apidoc.element.bytewise.equal"></a>[function <span class="apidocSignatureSpan">bytewise.</span>equal (a, b)](#apidoc.element.bytewise.equal)
- description and source-code
```javascript
equal = function (a, b) {
  return base.compare(a, b) === 0
}
```
- example usage
```shell
...

'''js
var assert = require('assert');
var bytewise = require('./');
var encode = bytewise.encode;

// Many types can be represented using only their type tag, a single byte
assert.equal(encode(null).toString('binary'), '\x10');
assert.equal(encode(false).toString('binary'), '\x20');
assert.equal(encode(true).toString('binary'), '\x21');
assert.equal(encode(undefined).toString('binary'), '\xf0');

// Numbers are stored in 9 bytes -- 1 byte for the type tag and an 8 byte float
assert.equal(encode(12345).toString('hex'), '4240c81c8000000000');
// Negative numbers are stored as positive numbers, but with a lower type tag and their bits inverted
...
```

#### <a name="apidoc.element.bytewise.getType"></a>[function <span class="apidocSignatureSpan">bytewise.</span>getType (byte)](#apidoc.element.bytewise.getType)
- description and source-code
```javascript
getType = function (byte) {

  // construct and memoize byte prefix registry on first run
  if (!PREFIX_REGISTRY) {
    PREFIX_REGISTRY = {}

    // register sorts
    var sort
    for (var key in sorts) {
      sort = sorts[key]

      // if sort has subsorts register these instead
      sort.sorts ? registerTypes(sort.sorts) : registerType(sort)
    }
  }

  return PREFIX_REGISTRY[byte]
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bytewise.postDecode"></a>[function <span class="apidocSignatureSpan">bytewise.</span>postDecode (decoded, options)](#apidoc.element.bytewise.postDecode)
- description and source-code
```javascript
postDecode = function (decoded, options) {
  return decoded
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bytewise.postEncode"></a>[function <span class="apidocSignatureSpan">bytewise.</span>postEncode (encoded, options)](#apidoc.element.bytewise.postEncode)
- description and source-code
```javascript
postEncode = function (encoded, options) {

  // override buffer toString method to default to hex to help coercion issues
  // TODO: just return pure buffer, do this toString hackery in bytewise
  encoded.toString = function (encoding) {
    if (!encoding)
      return bytewise.stringCodec.decode(encoded)

    return Buffer.prototype.toString.apply(encoded, arguments)
  }

  return encoded
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bytewise.bound"></a>[module bytewise.bound](#apidoc.module.bytewise.bound)

#### <a name="apidoc.element.bytewise.bound.compare"></a>[function <span class="apidocSignatureSpan">bytewise.bound.</span>compare (a, b)](#apidoc.element.bytewise.bound.compare)
- description and source-code
```javascript
compare = function (a, b) {
  var aBound = base.bound.is(a)
  var bBound = base.bound.is(b)
  if (aBound) {
    if (bBound && !a.upper === !b.upper)
      return 0
    return a.upper ? 1 : -1
  }

  if (bBound)
    return -base.bound.compare(b, a)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bytewise.bound.encode"></a>[function <span class="apidocSignatureSpan">bytewise.bound.</span>encode (data, base)](#apidoc.element.bytewise.bound.encode)
- description and source-code
```javascript
encode = function (data, base) {
  return util.encodedBound(data, new Buffer([ data.upper ? 0xff : 0x00 ]))
}
```
- example usage
```shell
...


// TODO: encoding class hierarchy

var core = require('./binary')

exports.encode = function (source) {
  return core.encode(source).toString('hex')
}

exports.decode = function (buffer) {
  return core.decode(buffer.toString('hex'))
}

exports.buffer = false;
...
```

#### <a name="apidoc.element.bytewise.bound.getBoundary"></a>[function <span class="apidocSignatureSpan">bytewise.bound.</span>getBoundary (source)](#apidoc.element.bytewise.bound.getBoundary)
- description and source-code
```javascript
getBoundary = function (source) {
  return source instanceof BoundedKey && source.bound
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bytewise.bound.sort"></a>[module bytewise.bound.sort](#apidoc.module.bytewise.bound.sort)

#### <a name="apidoc.element.bytewise.bound.sort.compare"></a>[function <span class="apidocSignatureSpan">bytewise.bound.sort.</span>compare (a, b)](#apidoc.element.bytewise.bound.sort.compare)
- description and source-code
```javascript
compare = function (a, b) {
  //
  // test for invalid values
  //
  if (base.invalid(a, b))
    return NaN

  //
  // short circuit for identical objects
  //
  if (a === b)
    return 0

  //
  // short circuit for base bound types
  //
  var result = base.bound.compare(a, b)
  if (result !== undefined)
    return result

  //
  // cache typeof and valueOf for both values
  //
  var aTypeOf = typeof a
  var bTypeOf = typeof b
  var aValueOf = _valueOf(a)
  var bValueOf = _valueOf(b)

  //
  // loop over type tags and attempt compare
  //
  var order = base.order
  var sorts = base.sorts
  var sort
  for (var i = 0, length = order.length; i < length; ++i) {
    sort = sorts[order[i]]

    //
    // if first arg is a member of this sort we have an answer
    //
    if (sort.is(a, aTypeOf))
      //
      // if b is the same as a then defer to sort's comparator, else a comes first
      //
      return sort.is(b, bTypeOf) ? sort.compare(aValueOf, bValueOf) : -1

    //
    // if b is this type but not a then b comes first
    //
    if (sort.is(b, bTypeOf))
      return 1
  }

  //
  // values are incomparable as they didn't match against any registered types
  //
  return NaN
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bytewise.bound.sort.equal"></a>[function <span class="apidocSignatureSpan">bytewise.bound.sort.</span>equal (a, b)](#apidoc.element.bytewise.bound.sort.equal)
- description and source-code
```javascript
equal = function (a, b) {
  return base.compare(a, b) === 0
}
```
- example usage
```shell
...

'''js
var assert = require('assert');
var bytewise = require('./');
var encode = bytewise.encode;

// Many types can be represented using only their type tag, a single byte
assert.equal(encode(null).toString('binary'), '\x10');
assert.equal(encode(false).toString('binary'), '\x20');
assert.equal(encode(true).toString('binary'), '\x21');
assert.equal(encode(undefined).toString('binary'), '\xf0');

// Numbers are stored in 9 bytes -- 1 byte for the type tag and an 8 byte float
assert.equal(encode(12345).toString('hex'), '4240c81c8000000000');
// Negative numbers are stored as positive numbers, but with a lower type tag and their bits inverted
...
```

#### <a name="apidoc.element.bytewise.bound.sort.invalid"></a>[function <span class="apidocSignatureSpan">bytewise.bound.sort.</span>invalid (a, b)](#apidoc.element.bytewise.bound.sort.invalid)
- description and source-code
```javascript
invalid = function (a, b) {
  var types = base.invalid
  for (var key in types) {
    var type = types[key]
    if (type && type.is && (type.is(a) || type.is(b)))
      return true
  }
  return false
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bytewise.hex"></a>[module bytewise.hex](#apidoc.module.bytewise.hex)

#### <a name="apidoc.element.bytewise.hex.decode"></a>[function <span class="apidocSignatureSpan">bytewise.hex.</span>decode (buffer)](#apidoc.element.bytewise.hex.decode)
- description and source-code
```javascript
decode = function (buffer) {
  return core.decode(buffer.toString('hex'))
}
```
- example usage
```shell
...
var core = require('./binary')

exports.encode = function (source) {
  return core.encode(source).toString('hex')
}

exports.decode = function (buffer) {
  return core.decode(buffer.toString('hex'))
}

exports.buffer = false;
exports.type = 'bytewise-hex';
...
```

#### <a name="apidoc.element.bytewise.hex.encode"></a>[function <span class="apidocSignatureSpan">bytewise.hex.</span>encode (source)](#apidoc.element.bytewise.hex.encode)
- description and source-code
```javascript
encode = function (source) {
  return core.encode(source).toString('hex')
}
```
- example usage
```shell
...


// TODO: encoding class hierarchy

var core = require('./binary')

exports.encode = function (source) {
  return core.encode(source).toString('hex')
}

exports.decode = function (buffer) {
  return core.decode(buffer.toString('hex'))
}

exports.buffer = false;
...
```



# <a name="apidoc.module.bytewise.stringCodec"></a>[module bytewise.stringCodec](#apidoc.module.bytewise.stringCodec)

#### <a name="apidoc.element.bytewise.stringCodec.decode"></a>[function <span class="apidocSignatureSpan">bytewise.stringCodec.</span>decode (buffer)](#apidoc.element.bytewise.stringCodec.decode)
- description and source-code
```javascript
decode = function (buffer) {
  return buffer.toString('hex')
}
```
- example usage
```shell
...
var core = require('./binary')

exports.encode = function (source) {
  return core.encode(source).toString('hex')
}

exports.decode = function (buffer) {
  return core.decode(buffer.toString('hex'))
}

exports.buffer = false;
exports.type = 'bytewise-hex';
...
```

#### <a name="apidoc.element.bytewise.stringCodec.encode"></a>[function <span class="apidocSignatureSpan">bytewise.stringCodec.</span>encode (source)](#apidoc.element.bytewise.stringCodec.encode)
- description and source-code
```javascript
encode = function (source) {
  return new Buffer(source, 'hex')
}
```
- example usage
```shell
...


// TODO: encoding class hierarchy

var core = require('./binary')

exports.encode = function (source) {
  return core.encode(source).toString('hex')
}

exports.decode = function (buffer) {
  return core.decode(buffer.toString('hex'))
}

exports.buffer = false;
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
