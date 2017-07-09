This package is a express middleware what allows you to obfuscate javascript files and cache them.

[![npm version](https://badge.fury.io/js/express-middleware-obfuscator.svg)](https://www.npmjs.com/package/express-middleware-obfuscator) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Installation

```sh
npm i -S express-middleware-obfuscator
```

## Usage

```js
const express = require('express');
const app = express();

const express_middleware_obfuscator = require("express-middleware-obfuscator");

app.use(express_middleware_obfuscator({
    src: `${__dirname}/public`,
    version: 'alpha'
}));

app.listen(80);
```

### Example of obfuscation

#### Not obfuscated
```js
const helloMessage = (name = "undefined") => {
    console.log("Hello " + name)
};

const house = {
    name: "Casa topo",

    rooms: 3,
    bathrooms: 2,
    meters: 54,
    wooden_planks_floor: true,
    sell: () => {
        setInterval(() => {
            console.error(`${house.name} is now sold.`)
        }, 3000);
    },
    hi: () => {
        helloMessage(house.name);
    }
};

house.sell();
```

#### Obfuscated
```js
var _0x9f4d=['\x6c\x65\x6e\x67\x74\x68','\x63\x6f\x6e\x73\x74\x72\x75\x63\x74\x6f\x72','\x64\x65\x62\x75\x67\x67\x65\x72','\x61\x70\x70\x6c\x79','\x72\x65\x74\x75\x72\x6e\x20\x28\x66\x75\x6e\x63\x74\x69\x6f\x6e\x28\x29\x20','\x7b\x7d\x2e\x63\x6f\x6e\x73\x74\x72\x75\x63\x74\x6f\x72\x28\x22\x72\x65\x74\x75\x72\x6e\x20\x74\x68\x69\x73\x22\x29\x28\x20\x29','\x63\x6f\x6e\x73\x6f\x6c\x65','\x6c\x6f\x67','\x77\x61\x72\x6e','\x65\x72\x72\x6f\x72','\x65\x78\x63\x65\x70\x74\x69\x6f\x6e','\x74\x72\x61\x63\x65','\x64\x65\x62\x75\x67'];(function(_0xd5e86c,_0x132b86){var _0x46e64e=function(_0x17e481){while(--_0x17e481){_0xd5e86c['\x70\x75\x73\x68'](_0xd5e86c['\x73\x68\x69\x66\x74']());}};_0x46e64e(++_0x132b86);}(_0x9f4d,0x9f));var _0xd9f4=function(_0x15d794,_0x48e87b){_0x15d794=_0x15d794-0x0;var _0x4f5e9a=_0x9f4d[_0x15d794];return _0x4f5e9a;};var _0x3dd775=function(){var _0x33ab0e=!![];return function(_0x1ffa62,_0x5722de){var _0x11b3dc=_0x33ab0e?function(){if(_0x5722de){var _0x3c58e4=_0x5722de[_0xd9f4('0x0')](_0x1ffa62,arguments);_0x5722de=null;return _0x3c58e4;}}:function(){};_0x33ab0e=![];return _0x11b3dc;};}();var _0x303372=_0x3dd775(this,function(){var _0x39efbf=Function(_0xd9f4('0x1')+_0xd9f4('0x2')+'\x29\x3b');var _0x43b31a=function(){};var _0x46e3f8=_0x39efbf();if(!_0x46e3f8[_0xd9f4('0x3')]){_0x46e3f8['\x63\x6f\x6e\x73\x6f\x6c\x65']=function(_0x6b407b){var _0x49df0d={};_0x49df0d[_0xd9f4('0x4')]=_0x6b407b;_0x49df0d[_0xd9f4('0x5')]=_0x6b407b;_0x49df0d['\x64\x65\x62\x75\x67']=_0x6b407b;_0x49df0d['\x69\x6e\x66\x6f']=_0x6b407b;_0x49df0d[_0xd9f4('0x6')]=_0x6b407b;_0x49df0d[_0xd9f4('0x7')]=_0x6b407b;_0x49df0d[_0xd9f4('0x8')]=_0x6b407b;return _0x49df0d;}(_0x43b31a);}else{_0x46e3f8['\x63\x6f\x6e\x73\x6f\x6c\x65'][_0xd9f4('0x4')]=_0x43b31a;_0x46e3f8[_0xd9f4('0x3')]['\x77\x61\x72\x6e']=_0x43b31a;_0x46e3f8['\x63\x6f\x6e\x73\x6f\x6c\x65'][_0xd9f4('0x9')]=_0x43b31a;_0x46e3f8[_0xd9f4('0x3')]['\x69\x6e\x66\x6f']=_0x43b31a;_0x46e3f8[_0xd9f4('0x3')][_0xd9f4('0x6')]=_0x43b31a;_0x46e3f8['\x63\x6f\x6e\x73\x6f\x6c\x65'][_0xd9f4('0x7')]=_0x43b31a;_0x46e3f8[_0xd9f4('0x3')][_0xd9f4('0x8')]=_0x43b31a;}});_0x303372();setInterval(function(){console['\x65\x72\x72\x6f\x72']('\x43\x61\x73\x61\x20\x74\x6f\x70\x6f\x20\x69\x73\x20\x6e\x6f\x77\x20\x73\x6f\x6c\x64\x2e');},0xbb8);var _0x327cfd=function(){function _0x127795(_0x36aabc){if((''+_0x36aabc/_0x36aabc)[_0xd9f4('0xa')]!==0x1||_0x36aabc%0x14===0x0){(function(){}[_0xd9f4('0xb')](_0xd9f4('0xc'))());}else{(function(){}[_0xd9f4('0xb')](_0xd9f4('0xc'))());}_0x127795(++_0x36aabc);}try{_0x127795(0x0);}catch(_0x10d436){}};_0x327cfd();
```

## Options

| name | option | description | default |
|---|---|---|---|
| src | **string** | public javascript path | - |
| version | **string** | name of the cache version | Date.now() |
| console_enabled | **boolean** | if console log is enabled | true |
