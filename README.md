# @zibuthe7j11/nisi-in-repellat <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![dependency status][5]][6]
[![dev dependency status][7]][8]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

Is this value a JS Typed Array? This module works cross-realm/iframe, does not depend on `instanceof` or mutable properties, and despite ES6 Symbol.toStringTag.

## Example

```js
var isTypedArray = require('@zibuthe7j11/nisi-in-repellat');
var assert = require('assert');

assert.equal(false, isTypedArray(undefined));
assert.equal(false, isTypedArray(null));
assert.equal(false, isTypedArray(false));
assert.equal(false, isTypedArray(true));
assert.equal(false, isTypedArray([]));
assert.equal(false, isTypedArray({}));
assert.equal(false, isTypedArray(/a/g));
assert.equal(false, isTypedArray(new RegExp('a', 'g')));
assert.equal(false, isTypedArray(new Date()));
assert.equal(false, isTypedArray(42));
assert.equal(false, isTypedArray(NaN));
assert.equal(false, isTypedArray(Infinity));
assert.equal(false, isTypedArray(new Number(42)));
assert.equal(false, isTypedArray('foo'));
assert.equal(false, isTypedArray(Object('foo')));
assert.equal(false, isTypedArray(function () {}));
assert.equal(false, isTypedArray(function* () {}));
assert.equal(false, isTypedArray(x => x * x));
assert.equal(false, isTypedArray([]));

assert.ok(isTypedArray(new Int8Array()));
assert.ok(isTypedArray(new Uint8Array()));
assert.ok(isTypedArray(new Uint8ClampedArray()));
assert.ok(isTypedArray(new Int16Array()));
assert.ok(isTypedArray(new Uint16Array()));
assert.ok(isTypedArray(new Int32Array()));
assert.ok(isTypedArray(new Uint32Array()));
assert.ok(isTypedArray(new Float32Array()));
assert.ok(isTypedArray(new Float64Array()));
assert.ok(isTypedArray(new BigInt64Array()));
assert.ok(isTypedArray(new BigUint64Array()));
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.org/package/@zibuthe7j11/nisi-in-repellat
[npm-version-svg]: https://versionbadg.es/inspect-js/@zibuthe7j11/nisi-in-repellat.svg
[deps-svg]: https://david-dm.org/inspect-js/@zibuthe7j11/nisi-in-repellat.svg
[deps-url]: https://david-dm.org/inspect-js/@zibuthe7j11/nisi-in-repellat
[dev-deps-svg]: https://david-dm.org/inspect-js/@zibuthe7j11/nisi-in-repellat/dev-status.svg
[dev-deps-url]: https://david-dm.org/inspect-js/@zibuthe7j11/nisi-in-repellat#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@zibuthe7j11/nisi-in-repellat.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@zibuthe7j11/nisi-in-repellat.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@zibuthe7j11/nisi-in-repellat.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@zibuthe7j11/nisi-in-repellat
[codecov-image]: https://codecov.io/gh/inspect-js/@zibuthe7j11/nisi-in-repellat/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/inspect-js/@zibuthe7j11/nisi-in-repellat/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/inspect-js/@zibuthe7j11/nisi-in-repellat
[actions-url]: https://github.com/zibuthe7j11/nisi-in-repellat/actions
