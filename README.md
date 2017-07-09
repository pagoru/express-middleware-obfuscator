[![npm version](https://badge.fury.io/js/express-middleware-obfuscator.svg)](https://www.npmjs.com/package/express-middleware-obfuscator) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)


## About

This package is a express middleware what allows you to obfuscate javascript files and cache them.

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
var _0xd330=['\x63\x6f\x6e\x73\x6f\x6c\x65','\x77\x61\x72\x6e',
'\x65\x72\x72\x6f\x72','\x74\x72\x61\x63\x65','\x6c\x6f\x67',
'\x64\x65\x62\x75\x67','\x69\x6e\x66\x6f',
'\x65\x78\x63\x65\x70\x74\x69\x6f\x6e','\x6c\x65\x6e\x67\x74\x68',
'\x63\x6f\x6e\x73\x74\x72\x75\x63\x74\x6f\x72',
'\x64\x65\x62\x75\x67\x67\x65\x72',
'\x72\x65\x74\x75\x72\x6e\x20\x28\x66\x75\x6e\x63\x74\x69\x6f\x6e\x28\x29\x20',
'\x7b\x7d\x2e\x63\x6f\x6e\x73\x74\x72\x75\x63\x74\x6f\x72\x28\x22\x72\x65\x74\x75\x72\x6e\x20\x74\x68\x69\x73\x22\x29\x28\x20\x29'];
(function(_0x3644b4,_0xa61af1){var _0x4a5169=function(_0x59afb6){
while(--_0x59afb6){_0x3644b4['\x70\x75\x73\x68'](_0x3644b4['\x73\x68\x69\x66\x74']());}};
_0x4a5169(++_0xa61af1);}(_0xd330,0x16a));
var _0x0d33=function(_0x2eca3e,_0x56fc6f){_0x2eca3e=_0x2eca3e-0x0;var
_0x10ca1d=_0xd330[_0x2eca3e];return _0x10ca1d;};var _0x423b3d=function(){
var _0x1c8529=!![];return function(_0x454d51,_0xda583f){
var _0x3628fd=_0x1c8529?function(){if(_0xda583f){
var _0x2743e9=_0xda583f['\x61\x70\x70\x6c\x79'](_0x454d51,arguments);_0xda583f=null;
return _0x2743e9;}}:function(){};_0x1c8529=![];return _0x3628fd;};}();
var _0x31c997=_0x423b3d(this,function(){var _0x4c7d40=
Function(_0x0d33('0x0')+_0x0d33('0x1')+'\x29\x3b');var _0xd5b153=
function(){};var _0x2df6b=_0x4c7d40();if(!_0x2df6b[_0x0d33('0x2')]){
_0x2df6b[_0x0d33('0x2')]=function(_0x4849ee){var _0x4ae4bb={};
_0x4ae4bb['\x6c\x6f\x67']=_0x4849ee;_0x4ae4bb[_0x0d33('0x3')]=_0x4849ee;
_0x4ae4bb['\x64\x65\x62\x75\x67']=_0x4849ee;_0x4ae4bb['\x69\x6e\x66\x6f']=_0x4849ee;
_0x4ae4bb[_0x0d33('0x4')]=_0x4849ee;_0x4ae4bb['\x65\x78\x63\x65\x70\x74\x69\x6f\x6e']=_0x4849ee;
_0x4ae4bb[_0x0d33('0x5')]=_0x4849ee;return _0x4ae4bb;}(_0xd5b153);
}else{_0x2df6b['\x63\x6f\x6e\x73\x6f\x6c\x65'][_0x0d33('0x6')]=_0xd5b153;
_0x2df6b[_0x0d33('0x2')][_0x0d33('0x3')]=_0xd5b153;_0x2df6b['\x63\x6f\x6e\x73\x6f\x6c\x65']
[_0x0d33('0x7')]=_0xd5b153;_0x2df6b[_0x0d33('0x2')][_0x0d33('0x8')]=_0xd5b153;
_0x2df6b[_0x0d33('0x2')][_0x0d33('0x4')]=_0xd5b153;_0x2df6b[_0x0d33('0x2')]
[_0x0d33('0x9')]=_0xd5b153;_0x2df6b[_0x0d33('0x2')][_0x0d33('0x5')]=_0xd5b153;}});
_0x31c997();setInterval(function(){console['\x65\x72\x72\x6f\x72']
('\x43\x61\x73\x61\x20\x74\x6f\x70\x6f\x20\x69\x73\x20\x6e\x6f\x77\x20\x73\x6f\x6c\x64\x2e');
},0xbb8);var _0x2430bf=function(){function _0x307db1(_0x9dc218){
if((''+_0x9dc218/_0x9dc218)[_0x0d33('0xa')]!==0x1||_0x9dc218%0x14===0x0)
{(function(){}[_0x0d33('0xb')]('\x64\x65\x62\x75\x67\x67\x65\x72')());
}else{(function(){}[_0x0d33('0xb')](_0x0d33('0xc'))());
}_0x307db1(++_0x9dc218);}try{_0x307db1(0x0);}catch(_0x2c5604){}};_0x2430bf();
```

## Options

| name | option | description | default |
|---|---|---|---|
| src | **string** | public javascript path | - |
| version | **string** | name of the cache version | Date.now() |
| console_enabled | **boolean** | if console log is enabled | true |