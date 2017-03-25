# api documentation for  [underscore (v1.8.3)](http://underscorejs.org)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-underscore.svg)](https://travis-ci.org/npmdoc/node-npmdoc-underscore)
#### JavaScript's functional programming helper library.

[![NPM](https://nodei.co/npm/underscore.png?downloads=true)](https://www.npmjs.com/package/underscore)

[![apidoc](https://npmdoc.github.io/node-npmdoc-underscore/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-underscore_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-underscore/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-underscore/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Jeremy Ashkenas",
        "email": "jeremy@documentcloud.org"
    },
    "bugs": {
        "url": "https://github.com/jashkenas/underscore/issues"
    },
    "dependencies": {},
    "description": "JavaScript's functional programming helper library.",
    "devDependencies": {
        "docco": "*",
        "eslint": "0.6.x",
        "karma": "~0.12.31",
        "karma-qunit": "~0.1.4",
        "qunit-cli": "~0.2.0",
        "uglify-js": "2.4.x"
    },
    "directories": {},
    "dist": {
        "shasum": "4f3fb53b106e6097fcf9cb4109f2a5e9bdfa5022",
        "tarball": "https://registry.npmjs.org/underscore/-/underscore-1.8.3.tgz"
    },
    "files": [
        "underscore.js",
        "underscore-min.js",
        "underscore-min.map",
        "LICENSE"
    ],
    "gitHead": "e4743ab712b8ab42ad4ccb48b155034d02394e4d",
    "homepage": "http://underscorejs.org",
    "keywords": [
        "util",
        "functional",
        "server",
        "client",
        "browser"
    ],
    "license": "MIT",
    "main": "underscore.js",
    "maintainers": [
        {
            "name": "jashkenas",
            "email": "jashkenas@gmail.com"
        }
    ],
    "name": "underscore",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/jashkenas/underscore.git"
    },
    "scripts": {
        "build": "uglifyjs underscore.js -c \"evaluate=false\" --comments \"/    .*/\" -m --source-map underscore-min.map -o underscore-min.js",
        "doc": "docco underscore.js",
        "lint": "eslint underscore.js test/*.js",
        "test": "npm run test-node && npm run lint",
        "test-browser": "npm i karma-phantomjs-launcher && ./node_modules/karma/bin/karma start",
        "test-node": "qunit-cli test/*.js"
    },
    "version": "1.8.3"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module underscore](#apidoc.module.underscore)
1.  [function <span class="apidocSignatureSpan">underscore.</span>_ (obj)](#apidoc.element.underscore._)
1.  [function <span class="apidocSignatureSpan">underscore.</span>after (times, func)](#apidoc.element.underscore.after)
1.  [function <span class="apidocSignatureSpan">underscore.</span>all (obj, predicate, context)](#apidoc.element.underscore.all)
1.  [function <span class="apidocSignatureSpan">underscore.</span>allKeys (obj)](#apidoc.element.underscore.allKeys)
1.  [function <span class="apidocSignatureSpan">underscore.</span>any (obj, predicate, context)](#apidoc.element.underscore.any)
1.  [function <span class="apidocSignatureSpan">underscore.</span>assign (obj)](#apidoc.element.underscore.assign)
1.  [function <span class="apidocSignatureSpan">underscore.</span>before (times, func)](#apidoc.element.underscore.before)
1.  [function <span class="apidocSignatureSpan">underscore.</span>bind (func, context)](#apidoc.element.underscore.bind)
1.  [function <span class="apidocSignatureSpan">underscore.</span>bindAll (obj)](#apidoc.element.underscore.bindAll)
1.  [function <span class="apidocSignatureSpan">underscore.</span>chain (obj)](#apidoc.element.underscore.chain)
1.  [function <span class="apidocSignatureSpan">underscore.</span>clone (obj)](#apidoc.element.underscore.clone)
1.  [function <span class="apidocSignatureSpan">underscore.</span>collect (obj, iteratee, context)](#apidoc.element.underscore.collect)
1.  [function <span class="apidocSignatureSpan">underscore.</span>compact (array)](#apidoc.element.underscore.compact)
1.  [function <span class="apidocSignatureSpan">underscore.</span>compose ()](#apidoc.element.underscore.compose)
1.  [function <span class="apidocSignatureSpan">underscore.</span>constant (value)](#apidoc.element.underscore.constant)
1.  [function <span class="apidocSignatureSpan">underscore.</span>contains (obj, item, fromIndex, guard)](#apidoc.element.underscore.contains)
1.  [function <span class="apidocSignatureSpan">underscore.</span>countBy (obj, iteratee, context)](#apidoc.element.underscore.countBy)
1.  [function <span class="apidocSignatureSpan">underscore.</span>create (prototype, props)](#apidoc.element.underscore.create)
1.  [function <span class="apidocSignatureSpan">underscore.</span>debounce (func, wait, immediate)](#apidoc.element.underscore.debounce)
1.  [function <span class="apidocSignatureSpan">underscore.</span>defaults (obj)](#apidoc.element.underscore.defaults)
1.  [function <span class="apidocSignatureSpan">underscore.</span>defer ()](#apidoc.element.underscore.defer)
1.  [function <span class="apidocSignatureSpan">underscore.</span>delay (func, wait)](#apidoc.element.underscore.delay)
1.  [function <span class="apidocSignatureSpan">underscore.</span>detect (obj, predicate, context)](#apidoc.element.underscore.detect)
1.  [function <span class="apidocSignatureSpan">underscore.</span>difference (array)](#apidoc.element.underscore.difference)
1.  [function <span class="apidocSignatureSpan">underscore.</span>drop (array, n, guard)](#apidoc.element.underscore.drop)
1.  [function <span class="apidocSignatureSpan">underscore.</span>each (obj, iteratee, context)](#apidoc.element.underscore.each)
1.  [function <span class="apidocSignatureSpan">underscore.</span>escape (string)](#apidoc.element.underscore.escape)
1.  [function <span class="apidocSignatureSpan">underscore.</span>every (obj, predicate, context)](#apidoc.element.underscore.every)
1.  [function <span class="apidocSignatureSpan">underscore.</span>extend (obj)](#apidoc.element.underscore.extend)
1.  [function <span class="apidocSignatureSpan">underscore.</span>extendOwn (obj)](#apidoc.element.underscore.extendOwn)
1.  [function <span class="apidocSignatureSpan">underscore.</span>filter (obj, predicate, context)](#apidoc.element.underscore.filter)
1.  [function <span class="apidocSignatureSpan">underscore.</span>find (obj, predicate, context)](#apidoc.element.underscore.find)
1.  [function <span class="apidocSignatureSpan">underscore.</span>findIndex (array, predicate, context)](#apidoc.element.underscore.findIndex)
1.  [function <span class="apidocSignatureSpan">underscore.</span>findKey (obj, predicate, context)](#apidoc.element.underscore.findKey)
1.  [function <span class="apidocSignatureSpan">underscore.</span>findLastIndex (array, predicate, context)](#apidoc.element.underscore.findLastIndex)
1.  [function <span class="apidocSignatureSpan">underscore.</span>findWhere (obj, attrs)](#apidoc.element.underscore.findWhere)
1.  [function <span class="apidocSignatureSpan">underscore.</span>first (array, n, guard)](#apidoc.element.underscore.first)
1.  [function <span class="apidocSignatureSpan">underscore.</span>flatten (array, shallow)](#apidoc.element.underscore.flatten)
1.  [function <span class="apidocSignatureSpan">underscore.</span>foldl (obj, iteratee, memo, context)](#apidoc.element.underscore.foldl)
1.  [function <span class="apidocSignatureSpan">underscore.</span>foldr (obj, iteratee, memo, context)](#apidoc.element.underscore.foldr)
1.  [function <span class="apidocSignatureSpan">underscore.</span>forEach (obj, iteratee, context)](#apidoc.element.underscore.forEach)
1.  [function <span class="apidocSignatureSpan">underscore.</span>functions (obj)](#apidoc.element.underscore.functions)
1.  [function <span class="apidocSignatureSpan">underscore.</span>groupBy (obj, iteratee, context)](#apidoc.element.underscore.groupBy)
1.  [function <span class="apidocSignatureSpan">underscore.</span>has (obj, key)](#apidoc.element.underscore.has)
1.  [function <span class="apidocSignatureSpan">underscore.</span>head (array, n, guard)](#apidoc.element.underscore.head)
1.  [function <span class="apidocSignatureSpan">underscore.</span>identity (value)](#apidoc.element.underscore.identity)
1.  [function <span class="apidocSignatureSpan">underscore.</span>include (obj, item, fromIndex, guard)](#apidoc.element.underscore.include)
1.  [function <span class="apidocSignatureSpan">underscore.</span>includes (obj, item, fromIndex, guard)](#apidoc.element.underscore.includes)
1.  [function <span class="apidocSignatureSpan">underscore.</span>indexBy (obj, iteratee, context)](#apidoc.element.underscore.indexBy)
1.  [function <span class="apidocSignatureSpan">underscore.</span>indexOf (array, item, idx)](#apidoc.element.underscore.indexOf)
1.  [function <span class="apidocSignatureSpan">underscore.</span>initial (array, n, guard)](#apidoc.element.underscore.initial)
1.  [function <span class="apidocSignatureSpan">underscore.</span>inject (obj, iteratee, memo, context)](#apidoc.element.underscore.inject)
1.  [function <span class="apidocSignatureSpan">underscore.</span>intersection (array)](#apidoc.element.underscore.intersection)
1.  [function <span class="apidocSignatureSpan">underscore.</span>invert (obj)](#apidoc.element.underscore.invert)
1.  [function <span class="apidocSignatureSpan">underscore.</span>invoke (obj, method)](#apidoc.element.underscore.invoke)
1.  [function <span class="apidocSignatureSpan">underscore.</span>isArguments (obj)](#apidoc.element.underscore.isArguments)
1.  [function <span class="apidocSignatureSpan">underscore.</span>isArray ()](#apidoc.element.underscore.isArray)
1.  [function <span class="apidocSignatureSpan">underscore.</span>isBoolean (obj)](#apidoc.element.underscore.isBoolean)
1.  [function <span class="apidocSignatureSpan">underscore.</span>isDate (obj)](#apidoc.element.underscore.isDate)
1.  [function <span class="apidocSignatureSpan">underscore.</span>isElement (obj)](#apidoc.element.underscore.isElement)
1.  [function <span class="apidocSignatureSpan">underscore.</span>isEmpty (obj)](#apidoc.element.underscore.isEmpty)
1.  [function <span class="apidocSignatureSpan">underscore.</span>isEqual (a, b)](#apidoc.element.underscore.isEqual)
1.  [function <span class="apidocSignatureSpan">underscore.</span>isError (obj)](#apidoc.element.underscore.isError)
1.  [function <span class="apidocSignatureSpan">underscore.</span>isFinite (obj)](#apidoc.element.underscore.isFinite)
1.  [function <span class="apidocSignatureSpan">underscore.</span>isFunction (obj)](#apidoc.element.underscore.isFunction)
1.  [function <span class="apidocSignatureSpan">underscore.</span>isMatch (object, attrs)](#apidoc.element.underscore.isMatch)
1.  [function <span class="apidocSignatureSpan">underscore.</span>isNaN (obj)](#apidoc.element.underscore.isNaN)
1.  [function <span class="apidocSignatureSpan">underscore.</span>isNull (obj)](#apidoc.element.underscore.isNull)
1.  [function <span class="apidocSignatureSpan">underscore.</span>isNumber (obj)](#apidoc.element.underscore.isNumber)
1.  [function <span class="apidocSignatureSpan">underscore.</span>isObject (obj)](#apidoc.element.underscore.isObject)
1.  [function <span class="apidocSignatureSpan">underscore.</span>isRegExp (obj)](#apidoc.element.underscore.isRegExp)
1.  [function <span class="apidocSignatureSpan">underscore.</span>isString (obj)](#apidoc.element.underscore.isString)
1.  [function <span class="apidocSignatureSpan">underscore.</span>isUndefined (obj)](#apidoc.element.underscore.isUndefined)
1.  [function <span class="apidocSignatureSpan">underscore.</span>iteratee (value, context)](#apidoc.element.underscore.iteratee)
1.  [function <span class="apidocSignatureSpan">underscore.</span>keys (obj)](#apidoc.element.underscore.keys)
1.  [function <span class="apidocSignatureSpan">underscore.</span>last (array, n, guard)](#apidoc.element.underscore.last)
1.  [function <span class="apidocSignatureSpan">underscore.</span>lastIndexOf (array, item, idx)](#apidoc.element.underscore.lastIndexOf)
1.  [function <span class="apidocSignatureSpan">underscore.</span>map (obj, iteratee, context)](#apidoc.element.underscore.map)
1.  [function <span class="apidocSignatureSpan">underscore.</span>mapObject (obj, iteratee, context)](#apidoc.element.underscore.mapObject)
1.  [function <span class="apidocSignatureSpan">underscore.</span>matcher (attrs)](#apidoc.element.underscore.matcher)
1.  [function <span class="apidocSignatureSpan">underscore.</span>matches (attrs)](#apidoc.element.underscore.matches)
1.  [function <span class="apidocSignatureSpan">underscore.</span>max (obj, iteratee, context)](#apidoc.element.underscore.max)
1.  [function <span class="apidocSignatureSpan">underscore.</span>memoize (func, hasher)](#apidoc.element.underscore.memoize)
1.  [function <span class="apidocSignatureSpan">underscore.</span>methods (obj)](#apidoc.element.underscore.methods)
1.  [function <span class="apidocSignatureSpan">underscore.</span>min (obj, iteratee, context)](#apidoc.element.underscore.min)
1.  [function <span class="apidocSignatureSpan">underscore.</span>mixin (obj)](#apidoc.element.underscore.mixin)
1.  [function <span class="apidocSignatureSpan">underscore.</span>negate (predicate)](#apidoc.element.underscore.negate)
1.  [function <span class="apidocSignatureSpan">underscore.</span>noConflict ()](#apidoc.element.underscore.noConflict)
1.  [function <span class="apidocSignatureSpan">underscore.</span>noop ()](#apidoc.element.underscore.noop)
1.  [function <span class="apidocSignatureSpan">underscore.</span>now ()](#apidoc.element.underscore.now)
1.  [function <span class="apidocSignatureSpan">underscore.</span>object (list, values)](#apidoc.element.underscore.object)
1.  [function <span class="apidocSignatureSpan">underscore.</span>omit (obj, iteratee, context)](#apidoc.element.underscore.omit)
1.  [function <span class="apidocSignatureSpan">underscore.</span>once ()](#apidoc.element.underscore.once)
1.  [function <span class="apidocSignatureSpan">underscore.</span>pairs (obj)](#apidoc.element.underscore.pairs)
1.  [function <span class="apidocSignatureSpan">underscore.</span>partial (func)](#apidoc.element.underscore.partial)
1.  [function <span class="apidocSignatureSpan">underscore.</span>partition (obj, predicate, context)](#apidoc.element.underscore.partition)
1.  [function <span class="apidocSignatureSpan">underscore.</span>pick (object, oiteratee, context)](#apidoc.element.underscore.pick)
1.  [function <span class="apidocSignatureSpan">underscore.</span>pluck (obj, key)](#apidoc.element.underscore.pluck)
1.  [function <span class="apidocSignatureSpan">underscore.</span>property (key)](#apidoc.element.underscore.property)
1.  [function <span class="apidocSignatureSpan">underscore.</span>propertyOf (obj)](#apidoc.element.underscore.propertyOf)
1.  [function <span class="apidocSignatureSpan">underscore.</span>random (min, max)](#apidoc.element.underscore.random)
1.  [function <span class="apidocSignatureSpan">underscore.</span>range (start, stop, step)](#apidoc.element.underscore.range)
1.  [function <span class="apidocSignatureSpan">underscore.</span>reduce (obj, iteratee, memo, context)](#apidoc.element.underscore.reduce)
1.  [function <span class="apidocSignatureSpan">underscore.</span>reduceRight (obj, iteratee, memo, context)](#apidoc.element.underscore.reduceRight)
1.  [function <span class="apidocSignatureSpan">underscore.</span>reject (obj, predicate, context)](#apidoc.element.underscore.reject)
1.  [function <span class="apidocSignatureSpan">underscore.</span>rest (array, n, guard)](#apidoc.element.underscore.rest)
1.  [function <span class="apidocSignatureSpan">underscore.</span>result (object, property, fallback)](#apidoc.element.underscore.result)
1.  [function <span class="apidocSignatureSpan">underscore.</span>sample (obj, n, guard)](#apidoc.element.underscore.sample)
1.  [function <span class="apidocSignatureSpan">underscore.</span>select (obj, predicate, context)](#apidoc.element.underscore.select)
1.  [function <span class="apidocSignatureSpan">underscore.</span>shuffle (obj)](#apidoc.element.underscore.shuffle)
1.  [function <span class="apidocSignatureSpan">underscore.</span>size (obj)](#apidoc.element.underscore.size)
1.  [function <span class="apidocSignatureSpan">underscore.</span>some (obj, predicate, context)](#apidoc.element.underscore.some)
1.  [function <span class="apidocSignatureSpan">underscore.</span>sortBy (obj, iteratee, context)](#apidoc.element.underscore.sortBy)
1.  [function <span class="apidocSignatureSpan">underscore.</span>sortedIndex (array, obj, iteratee, context)](#apidoc.element.underscore.sortedIndex)
1.  [function <span class="apidocSignatureSpan">underscore.</span>tail (array, n, guard)](#apidoc.element.underscore.tail)
1.  [function <span class="apidocSignatureSpan">underscore.</span>take (array, n, guard)](#apidoc.element.underscore.take)
1.  [function <span class="apidocSignatureSpan">underscore.</span>tap (obj, interceptor)](#apidoc.element.underscore.tap)
1.  [function <span class="apidocSignatureSpan">underscore.</span>template (text, settings, oldSettings)](#apidoc.element.underscore.template)
1.  [function <span class="apidocSignatureSpan">underscore.</span>throttle (func, wait, options)](#apidoc.element.underscore.throttle)
1.  [function <span class="apidocSignatureSpan">underscore.</span>times (n, iteratee, context)](#apidoc.element.underscore.times)
1.  [function <span class="apidocSignatureSpan">underscore.</span>toArray (obj)](#apidoc.element.underscore.toArray)
1.  [function <span class="apidocSignatureSpan">underscore.</span>unescape (string)](#apidoc.element.underscore.unescape)
1.  [function <span class="apidocSignatureSpan">underscore.</span>union ()](#apidoc.element.underscore.union)
1.  [function <span class="apidocSignatureSpan">underscore.</span>uniq (array, isSorted, iteratee, context)](#apidoc.element.underscore.uniq)
1.  [function <span class="apidocSignatureSpan">underscore.</span>unique (array, isSorted, iteratee, context)](#apidoc.element.underscore.unique)
1.  [function <span class="apidocSignatureSpan">underscore.</span>uniqueId (prefix)](#apidoc.element.underscore.uniqueId)
1.  [function <span class="apidocSignatureSpan">underscore.</span>unzip (array)](#apidoc.element.underscore.unzip)
1.  [function <span class="apidocSignatureSpan">underscore.</span>values (obj)](#apidoc.element.underscore.values)
1.  [function <span class="apidocSignatureSpan">underscore.</span>where (obj, attrs)](#apidoc.element.underscore.where)
1.  [function <span class="apidocSignatureSpan">underscore.</span>without (array)](#apidoc.element.underscore.without)
1.  [function <span class="apidocSignatureSpan">underscore.</span>wrap (func, wrapper)](#apidoc.element.underscore.wrap)
1.  [function <span class="apidocSignatureSpan">underscore.</span>zip ()](#apidoc.element.underscore.zip)
1.  object <span class="apidocSignatureSpan">underscore.</span>templateSettings
1.  string <span class="apidocSignatureSpan">underscore.</span>VERSION



# <a name="apidoc.module.underscore"></a>[module underscore](#apidoc.module.underscore)

#### <a name="apidoc.element.underscore._"></a>[function <span class="apidocSignatureSpan">underscore.</span>_ (obj)](#apidoc.element.underscore._)
- description and source-code
```javascript
_ = function (obj) {
  if (obj instanceof _) return obj;
  if (!(this instanceof _)) return new _(obj);
  this._wrapped = obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.after"></a>[function <span class="apidocSignatureSpan">underscore.</span>after (times, func)](#apidoc.element.underscore.after)
- description and source-code
```javascript
after = function (times, func) {
  return function() {
    if (--times < 1) {
      return func.apply(this, arguments);
    }
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.all"></a>[function <span class="apidocSignatureSpan">underscore.</span>all (obj, predicate, context)](#apidoc.element.underscore.all)
- description and source-code
```javascript
all = function (obj, predicate, context) {
  predicate = cb(predicate, context);
  var keys = !isArrayLike(obj) && _.keys(obj),
      length = (keys || obj).length;
  for (var index = 0; index < length; index++) {
    var currentKey = keys ? keys[index] : index;
    if (!predicate(obj[currentKey], currentKey, obj)) return false;
  }
  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.allKeys"></a>[function <span class="apidocSignatureSpan">underscore.</span>allKeys (obj)](#apidoc.element.underscore.allKeys)
- description and source-code
```javascript
allKeys = function (obj) {
  if (!_.isObject(obj)) return [];
  var keys = [];
  for (var key in obj) keys.push(key);
  // Ahem, IE < 9.
  if (hasEnumBug) collectNonEnumProps(obj, keys);
  return keys;
}
```
- example usage
```shell
...
};

// Return a copy of the object only containing the whitelisted properties.
_.pick = function(object, oiteratee, context) {
  var result = {}, obj = object, iteratee, keys;
  if (obj == null) return result;
  if (_.isFunction(oiteratee)) {
    keys = _.allKeys(obj);
    iteratee = optimizeCb(oiteratee, context);
  } else {
    keys = flatten(arguments, false, false, 1);
    iteratee = function(value, key, obj) { return key in obj; };
    obj = Object(obj);
  }
  for (var i = 0, length = keys.length; i < length; i++) {
...
```

#### <a name="apidoc.element.underscore.any"></a>[function <span class="apidocSignatureSpan">underscore.</span>any (obj, predicate, context)](#apidoc.element.underscore.any)
- description and source-code
```javascript
any = function (obj, predicate, context) {
  predicate = cb(predicate, context);
  var keys = !isArrayLike(obj) && _.keys(obj),
      length = (keys || obj).length;
  for (var index = 0; index < length; index++) {
    var currentKey = keys ? keys[index] : index;
    if (predicate(obj[currentKey], currentKey, obj)) return true;
  }
  return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.assign"></a>[function <span class="apidocSignatureSpan">underscore.</span>assign (obj)](#apidoc.element.underscore.assign)
- description and source-code
```javascript
assign = function (obj) {
  var length = arguments.length;
  if (length < 2 || obj == null) return obj;
  for (var index = 1; index < length; index++) {
    var source = arguments[index],
        keys = keysFunc(source),
        l = keys.length;
    for (var i = 0; i < l; i++) {
      var key = keys[i];
      if (!undefinedOnly || obj[key] === void 0) obj[key] = source[key];
    }
  }
  return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.before"></a>[function <span class="apidocSignatureSpan">underscore.</span>before (times, func)](#apidoc.element.underscore.before)
- description and source-code
```javascript
before = function (times, func) {
  var memo;
  return function() {
    if (--times > 0) {
      memo = func.apply(this, arguments);
    }
    if (times <= 1) func = null;
    return memo;
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.bind"></a>[function <span class="apidocSignatureSpan">underscore.</span>bind (func, context)](#apidoc.element.underscore.bind)
- description and source-code
```javascript
bind = function (func, context) {
  if (nativeBind && func.bind === nativeBind) return nativeBind.apply(func, slice.call(arguments, 1));
  if (!_.isFunction(func)) throw new TypeError('Bind must be called on a function');
  var args = slice.call(arguments, 2);
  var bound = function() {
    return executeBound(func, bound, context, this, args.concat(slice.call(arguments)));
  };
  return bound;
}
```
- example usage
```shell
...
// are the method names to be bound. Useful for ensuring that all callbacks
// defined on an object belong to it.
_.bindAll = function(obj) {
  var i, length = arguments.length, key;
  if (length <= 1) throw new Error('bindAll must be passed function names');
  for (i = 1; i < length; i++) {
    key = arguments[i];
    obj[key] = _.bind(obj[key], obj);
  }
  return obj;
};

// Memoize an expensive function by storing its results.
_.memoize = function(func, hasher) {
  var memoize = function(key) {
...
```

#### <a name="apidoc.element.underscore.bindAll"></a>[function <span class="apidocSignatureSpan">underscore.</span>bindAll (obj)](#apidoc.element.underscore.bindAll)
- description and source-code
```javascript
bindAll = function (obj) {
  var i, length = arguments.length, key;
  if (length <= 1) throw new Error('bindAll must be passed function names');
  for (i = 1; i < length; i++) {
    key = arguments[i];
    obj[key] = _.bind(obj[key], obj);
  }
  return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.chain"></a>[function <span class="apidocSignatureSpan">underscore.</span>chain (obj)](#apidoc.element.underscore.chain)
- description and source-code
```javascript
chain = function (obj) {
  var instance = _(obj);
  instance._chain = true;
  return instance;
}
```
- example usage
```shell
...
// ---------------
// If Underscore is called as a function, it returns a wrapped object that
// can be used OO-style. This wrapper holds altered versions of all the
// underscore functions. Wrapped objects may be chained.

// Helper function to continue chaining intermediate results.
var result = function(instance, obj) {
  return instance._chain ? _(obj).chain() : obj;
};

// Add your own custom functions to the Underscore object.
_.mixin = function(obj) {
  _.each(_.functions(obj), function(name) {
    var func = _[name] = obj[name];
    _.prototype[name] = function() {
...
```

#### <a name="apidoc.element.underscore.clone"></a>[function <span class="apidocSignatureSpan">underscore.</span>clone (obj)](#apidoc.element.underscore.clone)
- description and source-code
```javascript
clone = function (obj) {
  if (!_.isObject(obj)) return obj;
  return _.isArray(obj) ? obj.slice() : _.extend({}, obj);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.collect"></a>[function <span class="apidocSignatureSpan">underscore.</span>collect (obj, iteratee, context)](#apidoc.element.underscore.collect)
- description and source-code
```javascript
collect = function (obj, iteratee, context) {
  iteratee = cb(iteratee, context);
  var keys = !isArrayLike(obj) && _.keys(obj),
      length = (keys || obj).length,
      results = Array(length);
  for (var index = 0; index < length; index++) {
    var currentKey = keys ? keys[index] : index;
    results[index] = iteratee(obj[currentKey], currentKey, obj);
  }
  return results;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.compact"></a>[function <span class="apidocSignatureSpan">underscore.</span>compact (array)](#apidoc.element.underscore.compact)
- description and source-code
```javascript
compact = function (array) {
  return _.filter(array, _.identity);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.compose"></a>[function <span class="apidocSignatureSpan">underscore.</span>compose ()](#apidoc.element.underscore.compose)
- description and source-code
```javascript
compose = function () {
  var args = arguments;
  var start = args.length - 1;
  return function() {
    var i = start;
    var result = args[start].apply(this, arguments);
    while (i--) result = args[i].call(this, result);
    return result;
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.constant"></a>[function <span class="apidocSignatureSpan">underscore.</span>constant (value)](#apidoc.element.underscore.constant)
- description and source-code
```javascript
constant = function (value) {
  return function() {
    return value;
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.contains"></a>[function <span class="apidocSignatureSpan">underscore.</span>contains (obj, item, fromIndex, guard)](#apidoc.element.underscore.contains)
- description and source-code
```javascript
contains = function (obj, item, fromIndex, guard) {
  if (!isArrayLike(obj)) obj = _.values(obj);
  if (typeof fromIndex != 'number' || guard) fromIndex = 0;
  return _.indexOf(obj, item, fromIndex) >= 0;
}
```
- example usage
```shell
...
for (var i = 0, length = getLength(array); i < length; i++) {
  var value = array[i],
      computed = iteratee ? iteratee(value, i, array) : value;
  if (isSorted) {
    if (!i || seen !== computed) result.push(value);
    seen = computed;
  } else if (iteratee) {
    if (!_.contains(seen, computed)) {
      seen.push(computed);
      result.push(value);
    }
  } else if (!_.contains(result, value)) {
    result.push(value);
  }
}
...
```

#### <a name="apidoc.element.underscore.countBy"></a>[function <span class="apidocSignatureSpan">underscore.</span>countBy (obj, iteratee, context)](#apidoc.element.underscore.countBy)
- description and source-code
```javascript
countBy = function (obj, iteratee, context) {
  var result = {};
  iteratee = cb(iteratee, context);
  _.each(obj, function(value, index) {
    var key = iteratee(value, index, obj);
    behavior(result, value, key);
  });
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.create"></a>[function <span class="apidocSignatureSpan">underscore.</span>create (prototype, props)](#apidoc.element.underscore.create)
- description and source-code
```javascript
create = function (prototype, props) {
  var result = baseCreate(prototype);
  if (props) _.extendOwn(result, props);
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.debounce"></a>[function <span class="apidocSignatureSpan">underscore.</span>debounce (func, wait, immediate)](#apidoc.element.underscore.debounce)
- description and source-code
```javascript
debounce = function (func, wait, immediate) {
  var timeout, args, context, timestamp, result;

  var later = function() {
    var last = _.now() - timestamp;

    if (last < wait && last >= 0) {
      timeout = setTimeout(later, wait - last);
    } else {
      timeout = null;
      if (!immediate) {
        result = func.apply(context, args);
        if (!timeout) context = args = null;
      }
    }
  };

  return function() {
    context = this;
    args = arguments;
    timestamp = _.now();
    var callNow = immediate && !timeout;
    if (!timeout) timeout = setTimeout(later, wait);
    if (callNow) {
      result = func.apply(context, args);
      context = args = null;
    }

    return result;
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.defaults"></a>[function <span class="apidocSignatureSpan">underscore.</span>defaults (obj)](#apidoc.element.underscore.defaults)
- description and source-code
```javascript
defaults = function (obj) {
  var length = arguments.length;
  if (length < 2 || obj == null) return obj;
  for (var index = 1; index < length; index++) {
    var source = arguments[index],
        keys = keysFunc(source),
        l = keys.length;
    for (var i = 0; i < l; i++) {
      var key = keys[i];
      if (!undefinedOnly || obj[key] === void 0) obj[key] = source[key];
    }
  }
  return obj;
}
```
- example usage
```shell
...

  // JavaScript micro-templating, similar to John Resig's implementation.
  // Underscore templating handles arbitrary delimiters, preserves whitespace,
  // and correctly escapes quotes within interpolated code.
  // NB: 'oldSettings' only exists for backwards compatibility.
  _.template = function(text, settings, oldSettings) {
if (!settings && oldSettings) settings = oldSettings;
settings = _.defaults({}, settings, _.templateSettings);

// Combine delimiters into one regular expression via alternation.
var matcher = RegExp([
  (settings.escape || noMatch).source,
  (settings.interpolate || noMatch).source,
  (settings.evaluate || noMatch).source
].join('|') + '|$', 'g');
...
```

#### <a name="apidoc.element.underscore.defer"></a>[function <span class="apidocSignatureSpan">underscore.</span>defer ()](#apidoc.element.underscore.defer)
- description and source-code
```javascript
defer = function () {
  var position = 0, length = boundArgs.length;
  var args = Array(length);
  for (var i = 0; i < length; i++) {
    args[i] = boundArgs[i] === _ ? arguments[position++] : boundArgs[i];
  }
  while (position < arguments.length) args.push(arguments[position++]);
  return executeBound(func, bound, this, this, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.delay"></a>[function <span class="apidocSignatureSpan">underscore.</span>delay (func, wait)](#apidoc.element.underscore.delay)
- description and source-code
```javascript
delay = function (func, wait) {
  var args = slice.call(arguments, 2);
  return setTimeout(function(){
    return func.apply(null, args);
  }, wait);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.detect"></a>[function <span class="apidocSignatureSpan">underscore.</span>detect (obj, predicate, context)](#apidoc.element.underscore.detect)
- description and source-code
```javascript
detect = function (obj, predicate, context) {
  var key;
  if (isArrayLike(obj)) {
    key = _.findIndex(obj, predicate, context);
  } else {
    key = _.findKey(obj, predicate, context);
  }
  if (key !== void 0 && key !== -1) return obj[key];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.difference"></a>[function <span class="apidocSignatureSpan">underscore.</span>difference (array)](#apidoc.element.underscore.difference)
- description and source-code
```javascript
difference = function (array) {
  var rest = flatten(arguments, true, true, 1);
  return _.filter(array, function(value){
    return !_.contains(rest, value);
  });
}
```
- example usage
```shell
...
// Flatten out an array, either recursively (by default), or just one level.
_.flatten = function(array, shallow) {
  return flatten(array, shallow, false);
};

// Return a version of the array that does not contain the specified value(s).
_.without = function(array) {
  return _.difference(array, slice.call(arguments, 1));
};

// Produce a duplicate-free version of the array. If the array has already
// been sorted, you have the option of using a faster algorithm.
// Aliased as 'unique'.
_.uniq = _.unique = function(array, isSorted, iteratee, context) {
  if (!_.isBoolean(isSorted)) {
...
```

#### <a name="apidoc.element.underscore.drop"></a>[function <span class="apidocSignatureSpan">underscore.</span>drop (array, n, guard)](#apidoc.element.underscore.drop)
- description and source-code
```javascript
drop = function (array, n, guard) {
  return slice.call(array, n == null || guard ? 1 : n);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.each"></a>[function <span class="apidocSignatureSpan">underscore.</span>each (obj, iteratee, context)](#apidoc.element.underscore.each)
- description and source-code
```javascript
each = function (obj, iteratee, context) {
  iteratee = optimizeCb(iteratee, context);
  var i, length;
  if (isArrayLike(obj)) {
    for (i = 0, length = obj.length; i < length; i++) {
      iteratee(obj[i], i, obj);
    }
  } else {
    var keys = _.keys(obj);
    for (i = 0, length = keys.length; i < length; i++) {
      iteratee(obj[keys[i]], keys[i], obj);
    }
  }
  return obj;
}
```
- example usage
```shell
...
};

// Return all the elements that pass a truth test.
// Aliased as 'select'.
_.filter = _.select = function(obj, predicate, context) {
  var results = [];
  predicate = cb(predicate, context);
  _.each(obj, function(value, index, list) {
    if (predicate(value, index, list)) results.push(value);
  });
  return results;
};

// Return all the elements for which a truth test fails.
_.reject = function(obj, predicate, context) {
...
```

#### <a name="apidoc.element.underscore.escape"></a>[function <span class="apidocSignatureSpan">underscore.</span>escape (string)](#apidoc.element.underscore.escape)
- description and source-code
```javascript
escape = function (string) {
  string = string == null ? '' : '' + string;
  return testRegexp.test(string) ? string.replace(replaceRegexp, escaper) : string;
}
```
- example usage
```shell
...
    var index = 0;
    var source = "__p+='";
    text.replace(matcher, function(match, escape, interpolate, evaluate, offset) {
source += text.slice(index, offset).replace(escaper, escapeChar);
index = offset + match.length;

if (escape) {
  source += "'+\n((__t=(" + escape + "))==null?'':_.escape(__t))+\n'";
} else if (interpolate) {
  source += "'+\n((__t=(" + interpolate + "))==null?'':__t)+\n'";
} else if (evaluate) {
  source += "';\n" + evaluate + "\n__p+='";
}

// Adobe VMs need the match returned to produce the correct offest.
...
```

#### <a name="apidoc.element.underscore.every"></a>[function <span class="apidocSignatureSpan">underscore.</span>every (obj, predicate, context)](#apidoc.element.underscore.every)
- description and source-code
```javascript
every = function (obj, predicate, context) {
  predicate = cb(predicate, context);
  var keys = !isArrayLike(obj) && _.keys(obj),
      length = (keys || obj).length;
  for (var index = 0; index < length; index++) {
    var currentKey = keys ? keys[index] : index;
    if (!predicate(obj[currentKey], currentKey, obj)) return false;
  }
  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.extend"></a>[function <span class="apidocSignatureSpan">underscore.</span>extend (obj)](#apidoc.element.underscore.extend)
- description and source-code
```javascript
extend = function (obj) {
  var length = arguments.length;
  if (length < 2 || obj == null) return obj;
  for (var index = 1; index < length; index++) {
    var source = arguments[index],
        keys = keysFunc(source),
        l = keys.length;
    for (var i = 0; i < l; i++) {
      var key = keys[i];
      if (!undefinedOnly || obj[key] === void 0) obj[key] = source[key];
    }
  }
  return obj;
}
```
- example usage
```shell
...
  if (props) _.extendOwn(result, props);
  return result;
};

// Create a (shallow-cloned) duplicate of an object.
_.clone = function(obj) {
  if (!_.isObject(obj)) return obj;
  return _.isArray(obj) ? obj.slice() : _.extend({}, obj);
};

// Invokes interceptor with the obj, and then returns obj.
// The primary purpose of this method is to "tap into" a method chain, in
// order to perform operations on intermediate results within the chain.
_.tap = function(obj, interceptor) {
  interceptor(obj);
...
```

#### <a name="apidoc.element.underscore.extendOwn"></a>[function <span class="apidocSignatureSpan">underscore.</span>extendOwn (obj)](#apidoc.element.underscore.extendOwn)
- description and source-code
```javascript
extendOwn = function (obj) {
  var length = arguments.length;
  if (length < 2 || obj == null) return obj;
  for (var index = 1; index < length; index++) {
    var source = arguments[index],
        keys = keysFunc(source),
        l = keys.length;
    for (var i = 0; i < l; i++) {
      var key = keys[i];
      if (!undefinedOnly || obj[key] === void 0) obj[key] = source[key];
    }
  }
  return obj;
}
```
- example usage
```shell
...
_.defaults = createAssigner(_.allKeys, true);

// Creates an object that inherits from the given prototype object.
// If additional properties are provided then they will be added to the
// created object.
_.create = function(prototype, props) {
  var result = baseCreate(prototype);
  if (props) _.extendOwn(result, props);
  return result;
};

// Create a (shallow-cloned) duplicate of an object.
_.clone = function(obj) {
  if (!_.isObject(obj)) return obj;
  return _.isArray(obj) ? obj.slice() : _.extend({}, obj);
...
```

#### <a name="apidoc.element.underscore.filter"></a>[function <span class="apidocSignatureSpan">underscore.</span>filter (obj, predicate, context)](#apidoc.element.underscore.filter)
- description and source-code
```javascript
filter = function (obj, predicate, context) {
  var results = [];
  predicate = cb(predicate, context);
  _.each(obj, function(value, index, list) {
    if (predicate(value, index, list)) results.push(value);
  });
  return results;
}
```
- example usage
```shell
...
    if (predicate(value, index, list)) results.push(value);
  });
  return results;
};

// Return all the elements for which a truth test fails.
_.reject = function(obj, predicate, context) {
  return _.filter(obj, _.negate(cb(predicate)), context);
};

// Determine whether all of the elements match a truth test.
// Aliased as 'all'.
_.every = _.all = function(obj, predicate, context) {
  predicate = cb(predicate, context);
  var keys = !isArrayLike(obj) && _.keys(obj),
...
```

#### <a name="apidoc.element.underscore.find"></a>[function <span class="apidocSignatureSpan">underscore.</span>find (obj, predicate, context)](#apidoc.element.underscore.find)
- description and source-code
```javascript
find = function (obj, predicate, context) {
  var key;
  if (isArrayLike(obj)) {
    key = _.findIndex(obj, predicate, context);
  } else {
    key = _.findKey(obj, predicate, context);
  }
  if (key !== void 0 && key !== -1) return obj[key];
}
```
- example usage
```shell
...
_.where = function(obj, attrs) {
  return _.filter(obj, _.matcher(attrs));
};

// Convenience version of a common use case of 'find': getting the first object
// containing specific 'key:value' pairs.
_.findWhere = function(obj, attrs) {
  return _.find(obj, _.matcher(attrs));
};

// Return the maximum element (or element-based computation).
_.max = function(obj, iteratee, context) {
  var result = -Infinity, lastComputed = -Infinity,
      value, computed;
  if (iteratee == null && obj != null) {
...
```

#### <a name="apidoc.element.underscore.findIndex"></a>[function <span class="apidocSignatureSpan">underscore.</span>findIndex (array, predicate, context)](#apidoc.element.underscore.findIndex)
- description and source-code
```javascript
findIndex = function (array, predicate, context) {
  predicate = cb(predicate, context);
  var length = getLength(array);
  var index = dir > 0 ? 0 : length - 1;
  for (; index >= 0 && index < length; index += dir) {
    if (predicate(array[index], index, array)) return index;
  }
  return -1;
}
```
- example usage
```shell
...
// The right-associative version of reduce, also known as 'foldr'.
_.reduceRight = _.foldr = createReduce(-1);

// Return the first value which passes a truth test. Aliased as 'detect'.
_.find = _.detect = function(obj, predicate, context) {
  var key;
  if (isArrayLike(obj)) {
    key = _.findIndex(obj, predicate, context);
  } else {
    key = _.findKey(obj, predicate, context);
  }
  if (key !== void 0 && key !== -1) return obj[key];
};

// Return all the elements that pass a truth test.
...
```

#### <a name="apidoc.element.underscore.findKey"></a>[function <span class="apidocSignatureSpan">underscore.</span>findKey (obj, predicate, context)](#apidoc.element.underscore.findKey)
- description and source-code
```javascript
findKey = function (obj, predicate, context) {
  predicate = cb(predicate, context);
  var keys = _.keys(obj), key;
  for (var i = 0, length = keys.length; i < length; i++) {
    key = keys[i];
    if (predicate(obj[key], key, obj)) return key;
  }
}
```
- example usage
```shell
...

// Return the first value which passes a truth test. Aliased as 'detect'.
_.find = _.detect = function(obj, predicate, context) {
  var key;
  if (isArrayLike(obj)) {
    key = _.findIndex(obj, predicate, context);
  } else {
    key = _.findKey(obj, predicate, context);
  }
  if (key !== void 0 && key !== -1) return obj[key];
};

// Return all the elements that pass a truth test.
// Aliased as 'select'.
_.filter = _.select = function(obj, predicate, context) {
...
```

#### <a name="apidoc.element.underscore.findLastIndex"></a>[function <span class="apidocSignatureSpan">underscore.</span>findLastIndex (array, predicate, context)](#apidoc.element.underscore.findLastIndex)
- description and source-code
```javascript
findLastIndex = function (array, predicate, context) {
  predicate = cb(predicate, context);
  var length = getLength(array);
  var index = dir > 0 ? 0 : length - 1;
  for (; index >= 0 && index < length; index += dir) {
    if (predicate(array[index], index, array)) return index;
  }
  return -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.findWhere"></a>[function <span class="apidocSignatureSpan">underscore.</span>findWhere (obj, attrs)](#apidoc.element.underscore.findWhere)
- description and source-code
```javascript
findWhere = function (obj, attrs) {
  return _.find(obj, _.matcher(attrs));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.first"></a>[function <span class="apidocSignatureSpan">underscore.</span>first (array, n, guard)](#apidoc.element.underscore.first)
- description and source-code
```javascript
first = function (array, n, guard) {
  if (array == null) return void 0;
  if (n == null || guard) return array[0];
  return _.initial(array, array.length - n);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.flatten"></a>[function <span class="apidocSignatureSpan">underscore.</span>flatten (array, shallow)](#apidoc.element.underscore.flatten)
- description and source-code
```javascript
flatten = function (array, shallow) {
  return flatten(array, shallow, false);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.foldl"></a>[function <span class="apidocSignatureSpan">underscore.</span>foldl (obj, iteratee, memo, context)](#apidoc.element.underscore.foldl)
- description and source-code
```javascript
foldl = function (obj, iteratee, memo, context) {
  iteratee = optimizeCb(iteratee, context, 4);
  var keys = !isArrayLike(obj) && _.keys(obj),
      length = (keys || obj).length,
      index = dir > 0 ? 0 : length - 1;
  // Determine the initial value if none is provided.
  if (arguments.length < 3) {
    memo = obj[keys ? keys[index] : index];
    index += dir;
  }
  return iterator(obj, iteratee, memo, keys, index, length);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.foldr"></a>[function <span class="apidocSignatureSpan">underscore.</span>foldr (obj, iteratee, memo, context)](#apidoc.element.underscore.foldr)
- description and source-code
```javascript
foldr = function (obj, iteratee, memo, context) {
  iteratee = optimizeCb(iteratee, context, 4);
  var keys = !isArrayLike(obj) && _.keys(obj),
      length = (keys || obj).length,
      index = dir > 0 ? 0 : length - 1;
  // Determine the initial value if none is provided.
  if (arguments.length < 3) {
    memo = obj[keys ? keys[index] : index];
    index += dir;
  }
  return iterator(obj, iteratee, memo, keys, index, length);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.forEach"></a>[function <span class="apidocSignatureSpan">underscore.</span>forEach (obj, iteratee, context)](#apidoc.element.underscore.forEach)
- description and source-code
```javascript
forEach = function (obj, iteratee, context) {
  iteratee = optimizeCb(iteratee, context);
  var i, length;
  if (isArrayLike(obj)) {
    for (i = 0, length = obj.length; i < length; i++) {
      iteratee(obj[i], i, obj);
    }
  } else {
    var keys = _.keys(obj);
    for (i = 0, length = keys.length; i < length; i++) {
      iteratee(obj[keys[i]], keys[i], obj);
    }
  }
  return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.functions"></a>[function <span class="apidocSignatureSpan">underscore.</span>functions (obj)](#apidoc.element.underscore.functions)
- description and source-code
```javascript
functions = function (obj) {
  var names = [];
  for (var key in obj) {
    if (_.isFunction(obj[key])) names.push(key);
  }
  return names.sort();
}
```
- example usage
```shell
...
// Helper function to continue chaining intermediate results.
var result = function(instance, obj) {
  return instance._chain ? _(obj).chain() : obj;
};

// Add your own custom functions to the Underscore object.
_.mixin = function(obj) {
  _.each(_.functions(obj), function(name) {
    var func = _[name] = obj[name];
    _.prototype[name] = function() {
      var args = [this._wrapped];
      push.apply(args, arguments);
      return result(this, func.apply(_, args));
    };
  });
...
```

#### <a name="apidoc.element.underscore.groupBy"></a>[function <span class="apidocSignatureSpan">underscore.</span>groupBy (obj, iteratee, context)](#apidoc.element.underscore.groupBy)
- description and source-code
```javascript
groupBy = function (obj, iteratee, context) {
  var result = {};
  iteratee = cb(iteratee, context);
  _.each(obj, function(value, index) {
    var key = iteratee(value, index, obj);
    behavior(result, value, key);
  });
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.has"></a>[function <span class="apidocSignatureSpan">underscore.</span>has (obj, key)](#apidoc.element.underscore.has)
- description and source-code
```javascript
has = function (obj, key) {
  return obj != null && hasOwnProperty.call(obj, key);
}
```
- example usage
```shell
...
    return result;
  };
};

// Groups the object's values by a criterion. Pass either a string attribute
// to group by, or a function that returns the criterion.
_.groupBy = group(function(result, value, key) {
  if (_.has(result, key)) result[key].push(value); else result[key] = [value];
});

// Indexes the object's values by a criterion, similar to 'groupBy', but for
// when you know that your index values will be unique.
_.indexBy = group(function(result, value, key) {
  result[key] = value;
});
...
```

#### <a name="apidoc.element.underscore.head"></a>[function <span class="apidocSignatureSpan">underscore.</span>head (array, n, guard)](#apidoc.element.underscore.head)
- description and source-code
```javascript
head = function (array, n, guard) {
  if (array == null) return void 0;
  if (n == null || guard) return array[0];
  return _.initial(array, array.length - n);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.identity"></a>[function <span class="apidocSignatureSpan">underscore.</span>identity (value)](#apidoc.element.underscore.identity)
- description and source-code
```javascript
identity = function (value) {
  return value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.include"></a>[function <span class="apidocSignatureSpan">underscore.</span>include (obj, item, fromIndex, guard)](#apidoc.element.underscore.include)
- description and source-code
```javascript
include = function (obj, item, fromIndex, guard) {
  if (!isArrayLike(obj)) obj = _.values(obj);
  if (typeof fromIndex != 'number' || guard) fromIndex = 0;
  return _.indexOf(obj, item, fromIndex) >= 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.includes"></a>[function <span class="apidocSignatureSpan">underscore.</span>includes (obj, item, fromIndex, guard)](#apidoc.element.underscore.includes)
- description and source-code
```javascript
includes = function (obj, item, fromIndex, guard) {
  if (!isArrayLike(obj)) obj = _.values(obj);
  if (typeof fromIndex != 'number' || guard) fromIndex = 0;
  return _.indexOf(obj, item, fromIndex) >= 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.indexBy"></a>[function <span class="apidocSignatureSpan">underscore.</span>indexBy (obj, iteratee, context)](#apidoc.element.underscore.indexBy)
- description and source-code
```javascript
indexBy = function (obj, iteratee, context) {
  var result = {};
  iteratee = cb(iteratee, context);
  _.each(obj, function(value, index) {
    var key = iteratee(value, index, obj);
    behavior(result, value, key);
  });
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.indexOf"></a>[function <span class="apidocSignatureSpan">underscore.</span>indexOf (array, item, idx)](#apidoc.element.underscore.indexOf)
- description and source-code
```javascript
indexOf = function (array, item, idx) {
  var i = 0, length = getLength(array);
  if (typeof idx == 'number') {
    if (dir > 0) {
        i = idx >= 0 ? idx : Math.max(idx + length, i);
    } else {
        length = idx >= 0 ? Math.min(idx + 1, length) : idx + length + 1;
    }
  } else if (sortedIndex && idx && length) {
    idx = sortedIndex(array, item);
    return array[idx] === item ? idx : -1;
  }
  if (item !== item) {
    idx = predicateFind(slice.call(array, i, length), _.isNaN);
    return idx >= 0 ? idx + i : -1;
  }
  for (idx = dir > 0 ? i : length - 1; idx >= 0 && idx < length; idx += dir) {
    if (array[idx] === item) return idx;
  }
  return -1;
}
```
- example usage
```shell
...
};

// Determine if the array or object contains a given item (using '===').
// Aliased as 'includes' and 'include'.
_.contains = _.includes = _.include = function(obj, item, fromIndex, guard) {
  if (!isArrayLike(obj)) obj = _.values(obj);
  if (typeof fromIndex != 'number' || guard) fromIndex = 0;
  return _.indexOf(obj, item, fromIndex) >= 0;
};

// Invoke a method (with arguments) on every item in a collection.
_.invoke = function(obj, method) {
  var args = slice.call(arguments, 2);
  var isFunc = _.isFunction(method);
  return _.map(obj, function(value) {
...
```

#### <a name="apidoc.element.underscore.initial"></a>[function <span class="apidocSignatureSpan">underscore.</span>initial (array, n, guard)](#apidoc.element.underscore.initial)
- description and source-code
```javascript
initial = function (array, n, guard) {
  return slice.call(array, 0, Math.max(0, array.length - (n == null || guard ? 1 : n)));
}
```
- example usage
```shell
...

// Get the first element of an array. Passing **n** will return the first N
// values in the array. Aliased as 'head' and 'take'. The **guard** check
// allows it to work with '_.map'.
_.first = _.head = _.take = function(array, n, guard) {
  if (array == null) return void 0;
  if (n == null || guard) return array[0];
  return _.initial(array, array.length - n);
};

// Returns everything but the last entry of the array. Especially useful on
// the arguments object. Passing **n** will return all the values in
// the array, excluding the last N.
_.initial = function(array, n, guard) {
  return slice.call(array, 0, Math.max(0, array.length - (n == null || guard ? 1 : n)));
...
```

#### <a name="apidoc.element.underscore.inject"></a>[function <span class="apidocSignatureSpan">underscore.</span>inject (obj, iteratee, memo, context)](#apidoc.element.underscore.inject)
- description and source-code
```javascript
inject = function (obj, iteratee, memo, context) {
  iteratee = optimizeCb(iteratee, context, 4);
  var keys = !isArrayLike(obj) && _.keys(obj),
      length = (keys || obj).length,
      index = dir > 0 ? 0 : length - 1;
  // Determine the initial value if none is provided.
  if (arguments.length < 3) {
    memo = obj[keys ? keys[index] : index];
    index += dir;
  }
  return iterator(obj, iteratee, memo, keys, index, length);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.intersection"></a>[function <span class="apidocSignatureSpan">underscore.</span>intersection (array)](#apidoc.element.underscore.intersection)
- description and source-code
```javascript
intersection = function (array) {
  var result = [];
  var argsLength = arguments.length;
  for (var i = 0, length = getLength(array); i < length; i++) {
    var item = array[i];
    if (_.contains(result, item)) continue;
    for (var j = 1; j < argsLength; j++) {
      if (!_.contains(arguments[j], item)) break;
    }
    if (j === argsLength) result.push(item);
  }
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.invert"></a>[function <span class="apidocSignatureSpan">underscore.</span>invert (obj)](#apidoc.element.underscore.invert)
- description and source-code
```javascript
invert = function (obj) {
  var result = {};
  var keys = _.keys(obj);
  for (var i = 0, length = keys.length; i < length; i++) {
    result[obj[keys[i]]] = keys[i];
  }
  return result;
}
```
- example usage
```shell
...
  '&': '&amp;',
  '<': '&lt;',
  '>': '&gt;',
  '"': '&quot;',
  "'": '&#x27;',
  ''': '&#x60;'
};
var unescapeMap = _.invert(escapeMap);

// Functions for escaping and unescaping strings to/from HTML interpolation.
var createEscaper = function(map) {
  var escaper = function(match) {
    return map[match];
  };
  // Regexes for identifying a key that needs to be escaped
...
```

#### <a name="apidoc.element.underscore.invoke"></a>[function <span class="apidocSignatureSpan">underscore.</span>invoke (obj, method)](#apidoc.element.underscore.invoke)
- description and source-code
```javascript
invoke = function (obj, method) {
  var args = slice.call(arguments, 2);
  var isFunc = _.isFunction(method);
  return _.map(obj, function(value) {
    var func = isFunc ? method : value[method];
    return func == null ? func : func.apply(value, args);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.isArguments"></a>[function <span class="apidocSignatureSpan">underscore.</span>isArguments (obj)](#apidoc.element.underscore.isArguments)
- description and source-code
```javascript
isArguments = function (obj) {
  return toString.call(obj) === '[object ' + name + ']';
}
```
- example usage
```shell
...
};

// Internal implementation of a recursive 'flatten' function.
var flatten = function(input, shallow, strict, startIndex) {
  var output = [], idx = 0;
  for (var i = startIndex || 0, length = getLength(input); i < length; i++) {
    var value = input[i];
    if (isArrayLike(value) && (_.isArray(value) || _.isArguments(value))) {
      //flatten current level of array or arguments object
      if (!shallow) value = flatten(value, shallow, strict);
      var j = 0, len = value.length;
      output.length += len;
      while (j < len) {
        output[idx++] = value[j++];
      }
...
```

#### <a name="apidoc.element.underscore.isArray"></a>[function <span class="apidocSignatureSpan">underscore.</span>isArray ()](#apidoc.element.underscore.isArray)
- description and source-code
```javascript
function isArray() { [native code] }
```
- example usage
```shell
...
_.countBy = group(function(result, value, key) {
  if (_.has(result, key)) result[key]++; else result[key] = 1;
});

// Safely create a real, live array from anything iterable.
_.toArray = function(obj) {
  if (!obj) return [];
  if (_.isArray(obj)) return slice.call(obj);
  if (isArrayLike(obj)) return _.map(obj, _.identity);
  return _.values(obj);
};

// Return the number of elements in an object.
_.size = function(obj) {
  if (obj == null) return 0;
...
```

#### <a name="apidoc.element.underscore.isBoolean"></a>[function <span class="apidocSignatureSpan">underscore.</span>isBoolean (obj)](#apidoc.element.underscore.isBoolean)
- description and source-code
```javascript
isBoolean = function (obj) {
  return obj === true || obj === false || toString.call(obj) === '[object Boolean]';
}
```
- example usage
```shell
...
  return _.difference(array, slice.call(arguments, 1));
};

// Produce a duplicate-free version of the array. If the array has already
// been sorted, you have the option of using a faster algorithm.
// Aliased as 'unique'.
_.uniq = _.unique = function(array, isSorted, iteratee, context) {
  if (!_.isBoolean(isSorted)) {
    context = iteratee;
    iteratee = isSorted;
    isSorted = false;
  }
  if (iteratee != null) iteratee = cb(iteratee, context);
  var result = [];
  var seen = [];
...
```

#### <a name="apidoc.element.underscore.isDate"></a>[function <span class="apidocSignatureSpan">underscore.</span>isDate (obj)](#apidoc.element.underscore.isDate)
- description and source-code
```javascript
isDate = function (obj) {
  return toString.call(obj) === '[object ' + name + ']';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.isElement"></a>[function <span class="apidocSignatureSpan">underscore.</span>isElement (obj)](#apidoc.element.underscore.isElement)
- description and source-code
```javascript
isElement = function (obj) {
  return !!(obj && obj.nodeType === 1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.isEmpty"></a>[function <span class="apidocSignatureSpan">underscore.</span>isEmpty (obj)](#apidoc.element.underscore.isEmpty)
- description and source-code
```javascript
isEmpty = function (obj) {
  if (obj == null) return true;
  if (isArrayLike(obj) && (_.isArray(obj) || _.isString(obj) || _.isArguments(obj))) return obj.length === 0;
  return _.keys(obj).length === 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.isEqual"></a>[function <span class="apidocSignatureSpan">underscore.</span>isEqual (a, b)](#apidoc.element.underscore.isEqual)
- description and source-code
```javascript
isEqual = function (a, b) {
  return eq(a, b);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.isError"></a>[function <span class="apidocSignatureSpan">underscore.</span>isError (obj)](#apidoc.element.underscore.isError)
- description and source-code
```javascript
isError = function (obj) {
  return toString.call(obj) === '[object ' + name + ']';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.isFinite"></a>[function <span class="apidocSignatureSpan">underscore.</span>isFinite (obj)](#apidoc.element.underscore.isFinite)
- description and source-code
```javascript
isFinite = function (obj) {
  return isFinite(obj) && !isNaN(parseFloat(obj));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.isFunction"></a>[function <span class="apidocSignatureSpan">underscore.</span>isFunction (obj)](#apidoc.element.underscore.isFunction)
- description and source-code
```javascript
isFunction = function (obj) {
  return typeof obj == 'function' || false;
}
```
- example usage
```shell
...
};

// A mostly-internal function to generate callbacks that can be applied
// to each element in a collection, returning the desired result — either
// identity, an arbitrary callback, a property matcher, or a property accessor.
var cb = function(value, context, argCount) {
  if (value == null) return _.identity;
  if (_.isFunction(value)) return optimizeCb(value, context, argCount);
  if (_.isObject(value)) return _.matcher(value);
  return _.property(value);
};
_.iteratee = function(value, context) {
  return cb(value, context, Infinity);
};
...
```

#### <a name="apidoc.element.underscore.isMatch"></a>[function <span class="apidocSignatureSpan">underscore.</span>isMatch (object, attrs)](#apidoc.element.underscore.isMatch)
- description and source-code
```javascript
isMatch = function (object, attrs) {
  var keys = _.keys(attrs), length = keys.length;
  if (object == null) return !length;
  var obj = Object(object);
  for (var i = 0; i < length; i++) {
    var key = keys[i];
    if (attrs[key] !== obj[key] || !(key in obj)) return false;
  }
  return true;
}
```
- example usage
```shell
...
};

// Returns a predicate for checking whether an object has a given set of
// 'key:value' pairs.
_.matcher = _.matches = function(attrs) {
  attrs = _.extendOwn({}, attrs);
  return function(obj) {
    return _.isMatch(obj, attrs);
  };
};

// Run a function **n** times.
_.times = function(n, iteratee, context) {
  var accum = Array(Math.max(0, n));
  iteratee = optimizeCb(iteratee, context, 1);
...
```

#### <a name="apidoc.element.underscore.isNaN"></a>[function <span class="apidocSignatureSpan">underscore.</span>isNaN (obj)](#apidoc.element.underscore.isNaN)
- description and source-code
```javascript
isNaN = function (obj) {
  return _.isNumber(obj) && obj !== +obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.isNull"></a>[function <span class="apidocSignatureSpan">underscore.</span>isNull (obj)](#apidoc.element.underscore.isNull)
- description and source-code
```javascript
isNull = function (obj) {
  return obj === null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.isNumber"></a>[function <span class="apidocSignatureSpan">underscore.</span>isNumber (obj)](#apidoc.element.underscore.isNumber)
- description and source-code
```javascript
isNumber = function (obj) {
  return toString.call(obj) === '[object ' + name + ']';
}
```
- example usage
```shell
...
// Is a given object a finite number?
_.isFinite = function(obj) {
  return isFinite(obj) && !isNaN(parseFloat(obj));
};

// Is the given value 'NaN'? (NaN is the only number which does not equal itself).
_.isNaN = function(obj) {
  return _.isNumber(obj) && obj !== +obj;
};

// Is a given value a boolean?
_.isBoolean = function(obj) {
  return obj === true || obj === false || toString.call(obj) === '[object Boolean]';
};
...
```

#### <a name="apidoc.element.underscore.isObject"></a>[function <span class="apidocSignatureSpan">underscore.</span>isObject (obj)](#apidoc.element.underscore.isObject)
- description and source-code
```javascript
isObject = function (obj) {
  var type = typeof obj;
  return type === 'function' || type === 'object' && !!obj;
}
```
- example usage
```shell
...

// A mostly-internal function to generate callbacks that can be applied
// to each element in a collection, returning the desired result — either
// identity, an arbitrary callback, a property matcher, or a property accessor.
var cb = function(value, context, argCount) {
  if (value == null) return _.identity;
  if (_.isFunction(value)) return optimizeCb(value, context, argCount);
  if (_.isObject(value)) return _.matcher(value);
  return _.property(value);
};
_.iteratee = function(value, context) {
  return cb(value, context, Infinity);
};

// An internal function for creating assigner functions.
...
```

#### <a name="apidoc.element.underscore.isRegExp"></a>[function <span class="apidocSignatureSpan">underscore.</span>isRegExp (obj)](#apidoc.element.underscore.isRegExp)
- description and source-code
```javascript
isRegExp = function (obj) {
  return toString.call(obj) === '[object ' + name + ']';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.isString"></a>[function <span class="apidocSignatureSpan">underscore.</span>isString (obj)](#apidoc.element.underscore.isString)
- description and source-code
```javascript
isString = function (obj) {
  return toString.call(obj) === '[object ' + name + ']';
}
```
- example usage
```shell
...
  return eq(a, b);
};

// Is a given array, string, or object empty?
// An "empty" object has no enumerable own-properties.
_.isEmpty = function(obj) {
  if (obj == null) return true;
  if (isArrayLike(obj) && (_.isArray(obj) || _.isString(obj) || _.isArguments(obj))) return obj.length === 0;
  return _.keys(obj).length === 0;
};

// Is a given value a DOM element?
_.isElement = function(obj) {
  return !!(obj && obj.nodeType === 1);
};
...
```

#### <a name="apidoc.element.underscore.isUndefined"></a>[function <span class="apidocSignatureSpan">underscore.</span>isUndefined (obj)](#apidoc.element.underscore.isUndefined)
- description and source-code
```javascript
isUndefined = function (obj) {
  return obj === void 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.iteratee"></a>[function <span class="apidocSignatureSpan">underscore.</span>iteratee (value, context)](#apidoc.element.underscore.iteratee)
- description and source-code
```javascript
iteratee = function (value, context) {
  return cb(value, context, Infinity);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.keys"></a>[function <span class="apidocSignatureSpan">underscore.</span>keys (obj)](#apidoc.element.underscore.keys)
- description and source-code
```javascript
keys = function (obj) {
  if (!_.isObject(obj)) return [];
  if (nativeKeys) return nativeKeys(obj);
  var keys = [];
  for (var key in obj) if (_.has(obj, key)) keys.push(key);
  // Ahem, IE < 9.
  if (hasEnumBug) collectNonEnumProps(obj, keys);
  return keys;
}
```
- example usage
```shell
...
  iteratee = optimizeCb(iteratee, context);
  var i, length;
  if (isArrayLike(obj)) {
    for (i = 0, length = obj.length; i < length; i++) {
      iteratee(obj[i], i, obj);
    }
  } else {
    var keys = _.keys(obj);
    for (i = 0, length = keys.length; i < length; i++) {
      iteratee(obj[keys[i]], keys[i], obj);
    }
  }
  return obj;
};
...
```

#### <a name="apidoc.element.underscore.last"></a>[function <span class="apidocSignatureSpan">underscore.</span>last (array, n, guard)](#apidoc.element.underscore.last)
- description and source-code
```javascript
last = function (array, n, guard) {
  if (array == null) return void 0;
  if (n == null || guard) return array[array.length - 1];
  return _.rest(array, Math.max(0, array.length - n));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.lastIndexOf"></a>[function <span class="apidocSignatureSpan">underscore.</span>lastIndexOf (array, item, idx)](#apidoc.element.underscore.lastIndexOf)
- description and source-code
```javascript
lastIndexOf = function (array, item, idx) {
  var i = 0, length = getLength(array);
  if (typeof idx == 'number') {
    if (dir > 0) {
        i = idx >= 0 ? idx : Math.max(idx + length, i);
    } else {
        length = idx >= 0 ? Math.min(idx + 1, length) : idx + length + 1;
    }
  } else if (sortedIndex && idx && length) {
    idx = sortedIndex(array, item);
    return array[idx] === item ? idx : -1;
  }
  if (item !== item) {
    idx = predicateFind(slice.call(array, i, length), _.isNaN);
    return idx >= 0 ? idx + i : -1;
  }
  for (idx = dir > 0 ? i : length - 1; idx >= 0 && idx < length; idx += dir) {
    if (array[idx] === item) return idx;
  }
  return -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.map"></a>[function <span class="apidocSignatureSpan">underscore.</span>map (obj, iteratee, context)](#apidoc.element.underscore.map)
- description and source-code
```javascript
map = function (obj, iteratee, context) {
  iteratee = cb(iteratee, context);
  var keys = !isArrayLike(obj) && _.keys(obj),
      length = (keys || obj).length,
      results = Array(length);
  for (var index = 0; index < length; index++) {
    var currentKey = keys ? keys[index] : index;
    results[index] = iteratee(obj[currentKey], currentKey, obj);
  }
  return results;
}
```
- example usage
```shell
...
  return _.indexOf(obj, item, fromIndex) >= 0;
};

// Invoke a method (with arguments) on every item in a collection.
_.invoke = function(obj, method) {
  var args = slice.call(arguments, 2);
  var isFunc = _.isFunction(method);
  return _.map(obj, function(value) {
    var func = isFunc ? method : value[method];
    return func == null ? func : func.apply(value, args);
  });
};

// Convenience version of a common use case of 'map': fetching a property.
_.pluck = function(obj, key) {
...
```

#### <a name="apidoc.element.underscore.mapObject"></a>[function <span class="apidocSignatureSpan">underscore.</span>mapObject (obj, iteratee, context)](#apidoc.element.underscore.mapObject)
- description and source-code
```javascript
mapObject = function (obj, iteratee, context) {
  iteratee = cb(iteratee, context);
  var keys =  _.keys(obj),
        length = keys.length,
        results = {},
        currentKey;
    for (var index = 0; index < length; index++) {
      currentKey = keys[index];
      results[currentKey] = iteratee(obj[currentKey], currentKey, obj);
    }
    return results;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.matcher"></a>[function <span class="apidocSignatureSpan">underscore.</span>matcher (attrs)](#apidoc.element.underscore.matcher)
- description and source-code
```javascript
matcher = function (attrs) {
  attrs = _.extendOwn({}, attrs);
  return function(obj) {
    return _.isMatch(obj, attrs);
  };
}
```
- example usage
```shell
...

// A mostly-internal function to generate callbacks that can be applied
// to each element in a collection, returning the desired result — either
// identity, an arbitrary callback, a property matcher, or a property accessor.
var cb = function(value, context, argCount) {
  if (value == null) return _.identity;
  if (_.isFunction(value)) return optimizeCb(value, context, argCount);
  if (_.isObject(value)) return _.matcher(value);
  return _.property(value);
};
_.iteratee = function(value, context) {
  return cb(value, context, Infinity);
};

// An internal function for creating assigner functions.
...
```

#### <a name="apidoc.element.underscore.matches"></a>[function <span class="apidocSignatureSpan">underscore.</span>matches (attrs)](#apidoc.element.underscore.matches)
- description and source-code
```javascript
matches = function (attrs) {
  attrs = _.extendOwn({}, attrs);
  return function(obj) {
    return _.isMatch(obj, attrs);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.max"></a>[function <span class="apidocSignatureSpan">underscore.</span>max (obj, iteratee, context)](#apidoc.element.underscore.max)
- description and source-code
```javascript
max = function (obj, iteratee, context) {
  var result = -Infinity, lastComputed = -Infinity,
      value, computed;
  if (iteratee == null && obj != null) {
    obj = isArrayLike(obj) ? obj : _.values(obj);
    for (var i = 0, length = obj.length; i < length; i++) {
      value = obj[i];
      if (value > result) {
        result = value;
      }
    }
  } else {
    iteratee = cb(iteratee, context);
    _.each(obj, function(value, index, list) {
      computed = iteratee(value, index, list);
      if (computed > lastComputed || computed === -Infinity && result === -Infinity) {
        result = value;
        lastComputed = computed;
      }
    });
  }
  return result;
}
```
- example usage
```shell
...
// If **n** is not specified, returns a single random element.
// The internal 'guard' argument allows it to work with 'map'.
_.sample = function(obj, n, guard) {
  if (n == null || guard) {
    if (!isArrayLike(obj)) obj = _.values(obj);
    return obj[_.random(obj.length - 1)];
  }
  return _.shuffle(obj).slice(0, Math.max(0, n));
};

// Sort the object's values by a criterion produced by an iteratee.
_.sortBy = function(obj, iteratee, context) {
  iteratee = cb(iteratee, context);
  return _.pluck(_.map(obj, function(value, index, list) {
    return {
...
```

#### <a name="apidoc.element.underscore.memoize"></a>[function <span class="apidocSignatureSpan">underscore.</span>memoize (func, hasher)](#apidoc.element.underscore.memoize)
- description and source-code
```javascript
memoize = function (func, hasher) {
  var memoize = function(key) {
    var cache = memoize.cache;
    var address = '' + (hasher ? hasher.apply(this, arguments) : key);
    if (!_.has(cache, address)) cache[address] = func.apply(this, arguments);
    return cache[address];
  };
  memoize.cache = {};
  return memoize;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.methods"></a>[function <span class="apidocSignatureSpan">underscore.</span>methods (obj)](#apidoc.element.underscore.methods)
- description and source-code
```javascript
methods = function (obj) {
  var names = [];
  for (var key in obj) {
    if (_.isFunction(obj[key])) names.push(key);
  }
  return names.sort();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.min"></a>[function <span class="apidocSignatureSpan">underscore.</span>min (obj, iteratee, context)](#apidoc.element.underscore.min)
- description and source-code
```javascript
min = function (obj, iteratee, context) {
  var result = Infinity, lastComputed = Infinity,
      value, computed;
  if (iteratee == null && obj != null) {
    obj = isArrayLike(obj) ? obj : _.values(obj);
    for (var i = 0, length = obj.length; i < length; i++) {
      value = obj[i];
      if (value < result) {
        result = value;
      }
    }
  } else {
    iteratee = cb(iteratee, context);
    _.each(obj, function(value, index, list) {
      computed = iteratee(value, index, list);
      if (computed < lastComputed || computed === Infinity && result === Infinity) {
        result = value;
        lastComputed = computed;
      }
    });
  }
  return result;
}
```
- example usage
```shell
...
  function createIndexFinder(dir, predicateFind, sortedIndex) {
return function(array, item, idx) {
  var i = 0, length = getLength(array);
  if (typeof idx == 'number') {
    if (dir > 0) {
        i = idx >= 0 ? idx : Math.max(idx + length, i);
    } else {
        length = idx >= 0 ? Math.min(idx + 1, length) : idx + length + 1;
    }
  } else if (sortedIndex && idx && length) {
    idx = sortedIndex(array, item);
    return array[idx] === item ? idx : -1;
  }
  if (item !== item) {
    idx = predicateFind(slice.call(array, i, length), _.isNaN);
...
```

#### <a name="apidoc.element.underscore.mixin"></a>[function <span class="apidocSignatureSpan">underscore.</span>mixin (obj)](#apidoc.element.underscore.mixin)
- description and source-code
```javascript
mixin = function (obj) {
  _.each(_.functions(obj), function(name) {
    var func = _[name] = obj[name];
    _.prototype[name] = function() {
      var args = [this._wrapped];
      push.apply(args, arguments);
      return result(this, func.apply(_, args));
    };
  });
}
```
- example usage
```shell
...
      push.apply(args, arguments);
      return result(this, func.apply(_, args));
    };
  });
};

// Add all of the Underscore functions to the wrapper object.
_.mixin(_);

// Add all mutator Array functions to the wrapper.
_.each(['pop', 'push', 'reverse', 'shift', 'sort', 'splice', 'unshift'], function(name) {
  var method = ArrayProto[name];
  _.prototype[name] = function() {
    var obj = this._wrapped;
    method.apply(obj, arguments);
...
```

#### <a name="apidoc.element.underscore.negate"></a>[function <span class="apidocSignatureSpan">underscore.</span>negate (predicate)](#apidoc.element.underscore.negate)
- description and source-code
```javascript
negate = function (predicate) {
  return function() {
    return !predicate.apply(this, arguments);
  };
}
```
- example usage
```shell
...
    if (predicate(value, index, list)) results.push(value);
  });
  return results;
};

// Return all the elements for which a truth test fails.
_.reject = function(obj, predicate, context) {
  return _.filter(obj, _.negate(cb(predicate)), context);
};

// Determine whether all of the elements match a truth test.
// Aliased as 'all'.
_.every = _.all = function(obj, predicate, context) {
  predicate = cb(predicate, context);
  var keys = !isArrayLike(obj) && _.keys(obj),
...
```

#### <a name="apidoc.element.underscore.noConflict"></a>[function <span class="apidocSignatureSpan">underscore.</span>noConflict ()](#apidoc.element.underscore.noConflict)
- description and source-code
```javascript
noConflict = function () {
  root._ = previousUnderscore;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.noop"></a>[function <span class="apidocSignatureSpan">underscore.</span>noop ()](#apidoc.element.underscore.noop)
- description and source-code
```javascript
noop = function (){}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.now"></a>[function <span class="apidocSignatureSpan">underscore.</span>now ()](#apidoc.element.underscore.now)
- description and source-code
```javascript
function now() { [native code] }
```
- example usage
```shell
...
// '{leading: false}'. To disable execution on the trailing edge, ditto.
_.throttle = function(func, wait, options) {
  var context, args, result;
  var timeout = null;
  var previous = 0;
  if (!options) options = {};
  var later = function() {
    previous = options.leading === false ? 0 : _.now();
    timeout = null;
    result = func.apply(context, args);
    if (!timeout) context = args = null;
  };
  return function() {
    var now = _.now();
    if (!previous && options.leading === false) previous = now;
...
```

#### <a name="apidoc.element.underscore.object"></a>[function <span class="apidocSignatureSpan">underscore.</span>object (list, values)](#apidoc.element.underscore.object)
- description and source-code
```javascript
object = function (list, values) {
  var result = {};
  for (var i = 0, length = getLength(list); i < length; i++) {
    if (values) {
      result[list[i]] = values[i];
    } else {
      result[list[i][0]] = list[i][1];
    }
  }
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.omit"></a>[function <span class="apidocSignatureSpan">underscore.</span>omit (obj, iteratee, context)](#apidoc.element.underscore.omit)
- description and source-code
```javascript
omit = function (obj, iteratee, context) {
  if (_.isFunction(iteratee)) {
    iteratee = _.negate(iteratee);
  } else {
    var keys = _.map(flatten(arguments, false, false, 1), String);
    iteratee = function(value, key) {
      return !_.contains(keys, key);
    };
  }
  return _.pick(obj, iteratee, context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.once"></a>[function <span class="apidocSignatureSpan">underscore.</span>once ()](#apidoc.element.underscore.once)
- description and source-code
```javascript
once = function () {
  var position = 0, length = boundArgs.length;
  var args = Array(length);
  for (var i = 0; i < length; i++) {
    args[i] = boundArgs[i] === _ ? arguments[position++] : boundArgs[i];
  }
  while (position < arguments.length) args.push(arguments[position++]);
  return executeBound(func, bound, this, this, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.pairs"></a>[function <span class="apidocSignatureSpan">underscore.</span>pairs (obj)](#apidoc.element.underscore.pairs)
- description and source-code
```javascript
pairs = function (obj) {
  var keys = _.keys(obj);
  var length = keys.length;
  var pairs = Array(length);
  for (var i = 0; i < length; i++) {
    pairs[i] = [keys[i], obj[keys[i]]];
  }
  return pairs;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.partial"></a>[function <span class="apidocSignatureSpan">underscore.</span>partial (func)](#apidoc.element.underscore.partial)
- description and source-code
```javascript
partial = function (func) {
  var boundArgs = slice.call(arguments, 1);
  var bound = function() {
    var position = 0, length = boundArgs.length;
    var args = Array(length);
    for (var i = 0; i < length; i++) {
      args[i] = boundArgs[i] === _ ? arguments[position++] : boundArgs[i];
    }
    while (position < arguments.length) args.push(arguments[position++]);
    return executeBound(func, bound, this, this, args);
  };
  return bound;
}
```
- example usage
```shell
...
  return setTimeout(function(){
    return func.apply(null, args);
  }, wait);
};

// Defers a function, scheduling it to run after the current call stack has
// cleared.
_.defer = _.partial(_.delay, _, 1);

// Returns a function, that, when invoked, will only be triggered at most once
// during a given window of time. Normally, the throttled function will run
// as much as it can, without ever going more than once per 'wait' duration;
// but if you'd like to disable the execution on the leading edge, pass
// '{leading: false}'. To disable execution on the trailing edge, ditto.
_.throttle = function(func, wait, options) {
...
```

#### <a name="apidoc.element.underscore.partition"></a>[function <span class="apidocSignatureSpan">underscore.</span>partition (obj, predicate, context)](#apidoc.element.underscore.partition)
- description and source-code
```javascript
partition = function (obj, predicate, context) {
  predicate = cb(predicate, context);
  var pass = [], fail = [];
  _.each(obj, function(value, key, obj) {
    (predicate(value, key, obj) ? pass : fail).push(value);
  });
  return [pass, fail];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.pick"></a>[function <span class="apidocSignatureSpan">underscore.</span>pick (object, oiteratee, context)](#apidoc.element.underscore.pick)
- description and source-code
```javascript
pick = function (object, oiteratee, context) {
  var result = {}, obj = object, iteratee, keys;
  if (obj == null) return result;
  if (_.isFunction(oiteratee)) {
    keys = _.allKeys(obj);
    iteratee = optimizeCb(oiteratee, context);
  } else {
    keys = flatten(arguments, false, false, 1);
    iteratee = function(value, key, obj) { return key in obj; };
    obj = Object(obj);
  }
  for (var i = 0, length = keys.length; i < length; i++) {
    var key = keys[i];
    var value = obj[key];
    if (iteratee(value, key, obj)) result[key] = value;
  }
  return result;
}
```
- example usage
```shell
...
    iteratee = _.negate(iteratee);
  } else {
    var keys = _.map(flatten(arguments, false, false, 1), String);
    iteratee = function(value, key) {
      return !_.contains(keys, key);
    };
  }
  return _.pick(obj, iteratee, context);
};

// Fill in a given object with default properties.
_.defaults = createAssigner(_.allKeys, true);

// Creates an object that inherits from the given prototype object.
// If additional properties are provided then they will be added to the
...
```

#### <a name="apidoc.element.underscore.pluck"></a>[function <span class="apidocSignatureSpan">underscore.</span>pluck (obj, key)](#apidoc.element.underscore.pluck)
- description and source-code
```javascript
pluck = function (obj, key) {
  return _.map(obj, _.property(key));
}
```
- example usage
```shell
...
  }
  return _.shuffle(obj).slice(0, Math.max(0, n));
};

// Sort the object's values by a criterion produced by an iteratee.
_.sortBy = function(obj, iteratee, context) {
  iteratee = cb(iteratee, context);
  return _.pluck(_.map(obj, function(value, index, list) {
    return {
      value: value,
      index: index,
      criteria: iteratee(value, index, list)
    };
  }).sort(function(left, right) {
    var a = left.criteria;
...
```

#### <a name="apidoc.element.underscore.property"></a>[function <span class="apidocSignatureSpan">underscore.</span>property (key)](#apidoc.element.underscore.property)
- description and source-code
```javascript
property = function (key) {
  return function(obj) {
    return obj == null ? void 0 : obj[key];
  };
}
```
- example usage
```shell
...
// A mostly-internal function to generate callbacks that can be applied
// to each element in a collection, returning the desired result — either
// identity, an arbitrary callback, a property matcher, or a property accessor.
var cb = function(value, context, argCount) {
  if (value == null) return _.identity;
  if (_.isFunction(value)) return optimizeCb(value, context, argCount);
  if (_.isObject(value)) return _.matcher(value);
  return _.property(value);
};
_.iteratee = function(value, context) {
  return cb(value, context, Infinity);
};

// An internal function for creating assigner functions.
var createAssigner = function(keysFunc, undefinedOnly) {
...
```

#### <a name="apidoc.element.underscore.propertyOf"></a>[function <span class="apidocSignatureSpan">underscore.</span>propertyOf (obj)](#apidoc.element.underscore.propertyOf)
- description and source-code
```javascript
propertyOf = function (obj) {
  return obj == null ? function(){} : function(key) {
    return obj[key];
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.random"></a>[function <span class="apidocSignatureSpan">underscore.</span>random (min, max)](#apidoc.element.underscore.random)
- description and source-code
```javascript
random = function (min, max) {
  if (max == null) {
    max = min;
    min = 0;
  }
  return min + Math.floor(Math.random() * (max - min + 1));
}
```
- example usage
```shell
...
// Shuffle a collection, using the modern version of the
// [Fisher-Yates shuffle](http://en.wikipedia.org/wiki/Fisher–Yates_shuffle).
_.shuffle = function(obj) {
  var set = isArrayLike(obj) ? obj : _.values(obj);
  var length = set.length;
  var shuffled = Array(length);
  for (var index = 0, rand; index < length; index++) {
    rand = _.random(0, index);
    if (rand !== index) shuffled[index] = shuffled[rand];
    shuffled[rand] = set[index];
  }
  return shuffled;
};

// Sample **n** random values from a collection.
...
```

#### <a name="apidoc.element.underscore.range"></a>[function <span class="apidocSignatureSpan">underscore.</span>range (start, stop, step)](#apidoc.element.underscore.range)
- description and source-code
```javascript
range = function (start, stop, step) {
  if (stop == null) {
    stop = start || 0;
    start = 0;
  }
  step = step || 1;

  var length = Math.max(Math.ceil((stop - start) / step), 0);
  var range = Array(length);

  for (var idx = 0; idx < length; idx++, start += step) {
    range[idx] = start;
  }

  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.reduce"></a>[function <span class="apidocSignatureSpan">underscore.</span>reduce (obj, iteratee, memo, context)](#apidoc.element.underscore.reduce)
- description and source-code
```javascript
reduce = function (obj, iteratee, memo, context) {
  iteratee = optimizeCb(iteratee, context, 4);
  var keys = !isArrayLike(obj) && _.keys(obj),
      length = (keys || obj).length,
      index = dir > 0 ? 0 : length - 1;
  // Determine the initial value if none is provided.
  if (arguments.length < 3) {
    memo = obj[keys ? keys[index] : index];
    index += dir;
  }
  return iterator(obj, iteratee, memo, keys, index, length);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.reduceRight"></a>[function <span class="apidocSignatureSpan">underscore.</span>reduceRight (obj, iteratee, memo, context)](#apidoc.element.underscore.reduceRight)
- description and source-code
```javascript
reduceRight = function (obj, iteratee, memo, context) {
  iteratee = optimizeCb(iteratee, context, 4);
  var keys = !isArrayLike(obj) && _.keys(obj),
      length = (keys || obj).length,
      index = dir > 0 ? 0 : length - 1;
  // Determine the initial value if none is provided.
  if (arguments.length < 3) {
    memo = obj[keys ? keys[index] : index];
    index += dir;
  }
  return iterator(obj, iteratee, memo, keys, index, length);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.reject"></a>[function <span class="apidocSignatureSpan">underscore.</span>reject (obj, predicate, context)](#apidoc.element.underscore.reject)
- description and source-code
```javascript
reject = function (obj, predicate, context) {
  return _.filter(obj, _.negate(cb(predicate)), context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.rest"></a>[function <span class="apidocSignatureSpan">underscore.</span>rest (array, n, guard)](#apidoc.element.underscore.rest)
- description and source-code
```javascript
rest = function (array, n, guard) {
  return slice.call(array, n == null || guard ? 1 : n);
}
```
- example usage
```shell
...
};

// Get the last element of an array. Passing **n** will return the last N
// values in the array.
_.last = function(array, n, guard) {
  if (array == null) return void 0;
  if (n == null || guard) return array[array.length - 1];
  return _.rest(array, Math.max(0, array.length - n));
};

// Returns everything but the first entry of the array. Aliased as 'tail' and 'drop'.
// Especially useful on the arguments object. Passing an **n** will return
// the rest N values in the array.
_.rest = _.tail = _.drop = function(array, n, guard) {
  return slice.call(array, n == null || guard ? 1 : n);
...
```

#### <a name="apidoc.element.underscore.result"></a>[function <span class="apidocSignatureSpan">underscore.</span>result (object, property, fallback)](#apidoc.element.underscore.result)
- description and source-code
```javascript
result = function (object, property, fallback) {
  var value = object == null ? void 0 : object[property];
  if (value === void 0) {
    value = fallback;
  }
  return _.isFunction(value) ? value.call(object) : value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.sample"></a>[function <span class="apidocSignatureSpan">underscore.</span>sample (obj, n, guard)](#apidoc.element.underscore.sample)
- description and source-code
```javascript
sample = function (obj, n, guard) {
  if (n == null || guard) {
    if (!isArrayLike(obj)) obj = _.values(obj);
    return obj[_.random(obj.length - 1)];
  }
  return _.shuffle(obj).slice(0, Math.max(0, n));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.select"></a>[function <span class="apidocSignatureSpan">underscore.</span>select (obj, predicate, context)](#apidoc.element.underscore.select)
- description and source-code
```javascript
select = function (obj, predicate, context) {
  var results = [];
  predicate = cb(predicate, context);
  _.each(obj, function(value, index, list) {
    if (predicate(value, index, list)) results.push(value);
  });
  return results;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.shuffle"></a>[function <span class="apidocSignatureSpan">underscore.</span>shuffle (obj)](#apidoc.element.underscore.shuffle)
- description and source-code
```javascript
shuffle = function (obj) {
  var set = isArrayLike(obj) ? obj : _.values(obj);
  var length = set.length;
  var shuffled = Array(length);
  for (var index = 0, rand; index < length; index++) {
    rand = _.random(0, index);
    if (rand !== index) shuffled[index] = shuffled[rand];
    shuffled[rand] = set[index];
  }
  return shuffled;
}
```
- example usage
```shell
...
// If **n** is not specified, returns a single random element.
// The internal 'guard' argument allows it to work with 'map'.
_.sample = function(obj, n, guard) {
  if (n == null || guard) {
    if (!isArrayLike(obj)) obj = _.values(obj);
    return obj[_.random(obj.length - 1)];
  }
  return _.shuffle(obj).slice(0, Math.max(0, n));
};

// Sort the object's values by a criterion produced by an iteratee.
_.sortBy = function(obj, iteratee, context) {
  iteratee = cb(iteratee, context);
  return _.pluck(_.map(obj, function(value, index, list) {
    return {
...
```

#### <a name="apidoc.element.underscore.size"></a>[function <span class="apidocSignatureSpan">underscore.</span>size (obj)](#apidoc.element.underscore.size)
- description and source-code
```javascript
size = function (obj) {
  if (obj == null) return 0;
  return isArrayLike(obj) ? obj.length : _.keys(obj).length;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.some"></a>[function <span class="apidocSignatureSpan">underscore.</span>some (obj, predicate, context)](#apidoc.element.underscore.some)
- description and source-code
```javascript
some = function (obj, predicate, context) {
  predicate = cb(predicate, context);
  var keys = !isArrayLike(obj) && _.keys(obj),
      length = (keys || obj).length;
  for (var index = 0; index < length; index++) {
    var currentKey = keys ? keys[index] : index;
    if (predicate(obj[currentKey], currentKey, obj)) return true;
  }
  return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.sortBy"></a>[function <span class="apidocSignatureSpan">underscore.</span>sortBy (obj, iteratee, context)](#apidoc.element.underscore.sortBy)
- description and source-code
```javascript
sortBy = function (obj, iteratee, context) {
  iteratee = cb(iteratee, context);
  return _.pluck(_.map(obj, function(value, index, list) {
    return {
      value: value,
      index: index,
      criteria: iteratee(value, index, list)
    };
  }).sort(function(left, right) {
    var a = left.criteria;
    var b = right.criteria;
    if (a !== b) {
      if (a > b || a === void 0) return 1;
      if (a < b || b === void 0) return -1;
    }
    return left.index - right.index;
  }), 'value');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.sortedIndex"></a>[function <span class="apidocSignatureSpan">underscore.</span>sortedIndex (array, obj, iteratee, context)](#apidoc.element.underscore.sortedIndex)
- description and source-code
```javascript
sortedIndex = function (array, obj, iteratee, context) {
  iteratee = cb(iteratee, context, 1);
  var value = iteratee(obj);
  var low = 0, high = getLength(array);
  while (low < high) {
    var mid = Math.floor((low + high) / 2);
    if (iteratee(array[mid]) < value) low = mid + 1; else high = mid;
  }
  return low;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.tail"></a>[function <span class="apidocSignatureSpan">underscore.</span>tail (array, n, guard)](#apidoc.element.underscore.tail)
- description and source-code
```javascript
tail = function (array, n, guard) {
  return slice.call(array, n == null || guard ? 1 : n);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.take"></a>[function <span class="apidocSignatureSpan">underscore.</span>take (array, n, guard)](#apidoc.element.underscore.take)
- description and source-code
```javascript
take = function (array, n, guard) {
  if (array == null) return void 0;
  if (n == null || guard) return array[0];
  return _.initial(array, array.length - n);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.tap"></a>[function <span class="apidocSignatureSpan">underscore.</span>tap (obj, interceptor)](#apidoc.element.underscore.tap)
- description and source-code
```javascript
tap = function (obj, interceptor) {
  interceptor(obj);
  return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.template"></a>[function <span class="apidocSignatureSpan">underscore.</span>template (text, settings, oldSettings)](#apidoc.element.underscore.template)
- description and source-code
```javascript
template = function (text, settings, oldSettings) {
  if (!settings && oldSettings) settings = oldSettings;
  settings = _.defaults({}, settings, _.templateSettings);

  // Combine delimiters into one regular expression via alternation.
  var matcher = RegExp([
    (settings.escape || noMatch).source,
    (settings.interpolate || noMatch).source,
    (settings.evaluate || noMatch).source
  ].join('|') + '|$', 'g');

  // Compile the template source, escaping string literals appropriately.
  var index = 0;
  var source = "__p+='";
  text.replace(matcher, function(match, escape, interpolate, evaluate, offset) {
    source += text.slice(index, offset).replace(escaper, escapeChar);
    index = offset + match.length;

    if (escape) {
      source += "'+\n((__t=(" + escape + "))==null?'':_.escape(__t))+\n'";
    } else if (interpolate) {
      source += "'+\n((__t=(" + interpolate + "))==null?'':__t)+\n'";
    } else if (evaluate) {
      source += "';\n" + evaluate + "\n__p+='";
    }

    // Adobe VMs need the match returned to produce the correct offest.
    return match;
  });
  source += "';\n";

  // If a variable is not specified, place data values in local scope.
  if (!settings.variable) source = 'with(obj||{}){\n' + source + '}\n';

  source = "var __t,__p='',__j=Array.prototype.join," +
    "print=function(){__p+=__j.call(arguments,'');};\n" +
    source + 'return __p;\n';

  try {
    var render = new Function(settings.variable || 'obj', '_', source);
  } catch (e) {
    e.source = source;
    throw e;
  }

  var template = function(data) {
    return render.call(this, data, _);
  };

  // Provide the compiled source as a convenience for precompilation.
  var argument = settings.variable || 'obj';
  template.source = 'function(' + argument + '){\n' + source + '}';

  return template;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.throttle"></a>[function <span class="apidocSignatureSpan">underscore.</span>throttle (func, wait, options)](#apidoc.element.underscore.throttle)
- description and source-code
```javascript
throttle = function (func, wait, options) {
  var context, args, result;
  var timeout = null;
  var previous = 0;
  if (!options) options = {};
  var later = function() {
    previous = options.leading === false ? 0 : _.now();
    timeout = null;
    result = func.apply(context, args);
    if (!timeout) context = args = null;
  };
  return function() {
    var now = _.now();
    if (!previous && options.leading === false) previous = now;
    var remaining = wait - (now - previous);
    context = this;
    args = arguments;
    if (remaining <= 0 || remaining > wait) {
      if (timeout) {
        clearTimeout(timeout);
        timeout = null;
      }
      previous = now;
      result = func.apply(context, args);
      if (!timeout) context = args = null;
    } else if (!timeout && options.trailing !== false) {
      timeout = setTimeout(later, remaining);
    }
    return result;
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.times"></a>[function <span class="apidocSignatureSpan">underscore.</span>times (n, iteratee, context)](#apidoc.element.underscore.times)
- description and source-code
```javascript
times = function (n, iteratee, context) {
  var accum = Array(Math.max(0, n));
  iteratee = optimizeCb(iteratee, context, 1);
  for (var i = 0; i < n; i++) accum[i] = iteratee(i);
  return accum;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.toArray"></a>[function <span class="apidocSignatureSpan">underscore.</span>toArray (obj)](#apidoc.element.underscore.toArray)
- description and source-code
```javascript
toArray = function (obj) {
  if (!obj) return [];
  if (_.isArray(obj)) return slice.call(obj);
  if (isArrayLike(obj)) return _.map(obj, _.identity);
  return _.values(obj);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.unescape"></a>[function <span class="apidocSignatureSpan">underscore.</span>unescape (string)](#apidoc.element.underscore.unescape)
- description and source-code
```javascript
unescape = function (string) {
  string = string == null ? '' : '' + string;
  return testRegexp.test(string) ? string.replace(replaceRegexp, escaper) : string;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.union"></a>[function <span class="apidocSignatureSpan">underscore.</span>union ()](#apidoc.element.underscore.union)
- description and source-code
```javascript
union = function () {
  return _.uniq(flatten(arguments, true, true));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.uniq"></a>[function <span class="apidocSignatureSpan">underscore.</span>uniq (array, isSorted, iteratee, context)](#apidoc.element.underscore.uniq)
- description and source-code
```javascript
uniq = function (array, isSorted, iteratee, context) {
  if (!_.isBoolean(isSorted)) {
    context = iteratee;
    iteratee = isSorted;
    isSorted = false;
  }
  if (iteratee != null) iteratee = cb(iteratee, context);
  var result = [];
  var seen = [];
  for (var i = 0, length = getLength(array); i < length; i++) {
    var value = array[i],
        computed = iteratee ? iteratee(value, i, array) : value;
    if (isSorted) {
      if (!i || seen !== computed) result.push(value);
      seen = computed;
    } else if (iteratee) {
      if (!_.contains(seen, computed)) {
        seen.push(computed);
        result.push(value);
      }
    } else if (!_.contains(result, value)) {
      result.push(value);
    }
  }
  return result;
}
```
- example usage
```shell
...
  }
  return result;
};

// Produce an array that contains the union: each distinct element from all of
// the passed-in arrays.
_.union = function() {
  return _.uniq(flatten(arguments, true, true));
};

// Produce an array that contains every item shared between all the
// passed-in arrays.
_.intersection = function(array) {
  var result = [];
  var argsLength = arguments.length;
...
```

#### <a name="apidoc.element.underscore.unique"></a>[function <span class="apidocSignatureSpan">underscore.</span>unique (array, isSorted, iteratee, context)](#apidoc.element.underscore.unique)
- description and source-code
```javascript
unique = function (array, isSorted, iteratee, context) {
  if (!_.isBoolean(isSorted)) {
    context = iteratee;
    iteratee = isSorted;
    isSorted = false;
  }
  if (iteratee != null) iteratee = cb(iteratee, context);
  var result = [];
  var seen = [];
  for (var i = 0, length = getLength(array); i < length; i++) {
    var value = array[i],
        computed = iteratee ? iteratee(value, i, array) : value;
    if (isSorted) {
      if (!i || seen !== computed) result.push(value);
      seen = computed;
    } else if (iteratee) {
      if (!_.contains(seen, computed)) {
        seen.push(computed);
        result.push(value);
      }
    } else if (!_.contains(result, value)) {
      result.push(value);
    }
  }
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.uniqueId"></a>[function <span class="apidocSignatureSpan">underscore.</span>uniqueId (prefix)](#apidoc.element.underscore.uniqueId)
- description and source-code
```javascript
uniqueId = function (prefix) {
  var id = ++idCounter + '';
  return prefix ? prefix + id : id;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.unzip"></a>[function <span class="apidocSignatureSpan">underscore.</span>unzip (array)](#apidoc.element.underscore.unzip)
- description and source-code
```javascript
unzip = function (array) {
  var length = array && _.max(array, getLength).length || 0;
  var result = Array(length);

  for (var index = 0; index < length; index++) {
    result[index] = _.pluck(array, index);
  }
  return result;
}
```
- example usage
```shell
...
    return !_.contains(rest, value);
  });
};

// Zip together multiple lists into a single array -- elements that share
// an index go together.
_.zip = function() {
  return _.unzip(arguments);
};

// Complement of _.zip. Unzip accepts an array of arrays and groups
// each array's elements on shared indices
_.unzip = function(array) {
  var length = array && _.max(array, getLength).length || 0;
  var result = Array(length);
...
```

#### <a name="apidoc.element.underscore.values"></a>[function <span class="apidocSignatureSpan">underscore.</span>values (obj)](#apidoc.element.underscore.values)
- description and source-code
```javascript
values = function (obj) {
  var keys = _.keys(obj);
  var length = keys.length;
  var values = Array(length);
  for (var i = 0; i < length; i++) {
    values[i] = obj[keys[i]];
  }
  return values;
}
```
- example usage
```shell
...
  }
  return false;
};

// Determine if the array or object contains a given item (using '===').
// Aliased as 'includes' and 'include'.
_.contains = _.includes = _.include = function(obj, item, fromIndex, guard) {
  if (!isArrayLike(obj)) obj = _.values(obj);
  if (typeof fromIndex != 'number' || guard) fromIndex = 0;
  return _.indexOf(obj, item, fromIndex) >= 0;
};

// Invoke a method (with arguments) on every item in a collection.
_.invoke = function(obj, method) {
  var args = slice.call(arguments, 2);
...
```

#### <a name="apidoc.element.underscore.where"></a>[function <span class="apidocSignatureSpan">underscore.</span>where (obj, attrs)](#apidoc.element.underscore.where)
- description and source-code
```javascript
where = function (obj, attrs) {
  return _.filter(obj, _.matcher(attrs));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.without"></a>[function <span class="apidocSignatureSpan">underscore.</span>without (array)](#apidoc.element.underscore.without)
- description and source-code
```javascript
without = function (array) {
  return _.difference(array, slice.call(arguments, 1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.wrap"></a>[function <span class="apidocSignatureSpan">underscore.</span>wrap (func, wrapper)](#apidoc.element.underscore.wrap)
- description and source-code
```javascript
wrap = function (func, wrapper) {
  return _.partial(wrapper, func);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.underscore.zip"></a>[function <span class="apidocSignatureSpan">underscore.</span>zip ()](#apidoc.element.underscore.zip)
- description and source-code
```javascript
zip = function () {
  return _.unzip(arguments);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
