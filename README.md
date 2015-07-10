# xml-objtree

This is a node.js port of the XML.ObjTree implementation from http://www.kawa.net/works/js/xml/objtree-e.html

## Install

```
npm install --save xml-objtree
```

## Usage

```js
var ObjTree = require('xml-objtree');
var objTree = new ObjTree();

var xml = [
    '<?xml version="1.0" encoding="UTF-8"?>',
    '<books>',
    '<book id="1">The Art of Computer Programming</book>',
    '<book id="2">Introduction to Algorithms</book>',
    '</books>',
].join('\n');

var json = objTree.parseXML(xml);
```
