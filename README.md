# node-alias

Mac OS aliases creation and reading from node.js

## Attention

This library does currently not handle the `book\0\0\0\0mark\0\0\0\0`-header. It only does manipulation on the raw alias data.

I intend to add something like `alias.create(target)`, `alias.write(buf, path)` and `alias.read(path)`.

## Installation

```sh
npm install macos-alias
```

## Usage

```javascript
var alias = require('macos-alias');
```

## API

### alias.decode(buf)

Decodes buffer `buf` and returns an object with info about the alias.

### alias.encode(info)

Encodes the `info`-object into an alias, returns a buffer.

## Tests

```sh
mocha
```
