react-native-logger-client
==========

A Logger that runs on the device is the same as the chrome console.

  [![NPM Version](https://img.shields.io/npm/v/react-native-logger-client.svg?style=flat)](https://www.npmjs.org/package/react-native-logger-client)
  [![npm](https://img.shields.io/npm/dm/react-native-logger-client.svg?style=flat)](https://www.npmjs.org/package/react-native-logger-client)
  [![Build Status](https://travis-ci.org/TossShinHwa/react-native-logger-client.svg?branch=master&style=flat)](https://travis-ci.org/TossShinHwa/react-native-logger-client)
  [![License](http://img.shields.io/npm/l/react-native-logger-client.svg?style=flat)](https://raw.githubusercontent.com/TossShinHwa/react-native-logger-client/master/LICENSE)

## Usage

1.Integrate into the root component

```js
render() {
  return (
    <View>
      <App />
      {/* Let it be at the top of the app */}
      <Logger />
    </View>
  );
}
```

2.Use it anywhere

```js
console.log('Hello, Logs!');
console.info('This is a message.');
console.warn('user limit reached.');
console.error('error: name is undefined.');
console.log([{a:1, b:2, c:3}, {a:"foo", b:false, c:undefined}]);
```

<img src="https://github.com/TossShinHwa/react-native-logger-client/blob/master/img/example1.png?raw=true" width="300">
<img src="https://github.com/TossShinHwa/react-native-logger-client/blob/master/img/example2.png?raw=true" width="300">

## API

It will automatically integrate with the console, when you use such as `console.log`, it will be output to the device.

The following features are currently integrated.

* Console
  * [x] log
  * [x] info
  * [x] warn
  * [x] error

## Installation

```js
npm install --save react-native-logger-client
```

## TODO
* [ ] Mini window can be dragged
* [ ] Mini window should be change color when log something
* [ ] Limit maximum line number
* [ ] Filter log by type
* [ ] Show timestamps
* [ ] Custom style output
* [ ] Run on server
