ng-trunk8
======

About
-----

**ng-trunk8** is angular directive for [trunk8](http://jrvis.com/trunk8/).

Install
-----
```shell
[npm|bower] install ng-trunk8 -S
```

Usage
-----
```js
angular.modaule('app', ['ng-trunk8'])

```

**Default**
```js
<div trunk8>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor.</div>
```

By default, trunk8 will add an ellipsis (`&hellip;`) after the truncated text.

**Custom Settings**
```js
<div trunk8="{fill:'[sninp]', side:'center', text: vm.text}"></div> // 
```

Settings
--------

* **fill** _(Default: '`&hellip;`')_ The string to insert in place of the omitted text. This value may include HTML.
* **lines** _(Default: `1`)_ The number of lines of text-wrap to tolerate before truncating. This value must be an integer greater than or equal to 1.
* **side** _(Default: `'right'`)_ The side of the text from which to truncate. Valid values include `'center'`, `'left'`, and `'right'`.
* **tooltip** _(Default: `true`)_ When true, the `title` attribute of the targeted HTML element will be set to the original, untruncated string. Valid values include `true` and `false`.
* **width** _(Default: `'auto'`)_ The width, in characters, of the desired text. When set to `'auto'`, trunk8 will maximize the amount of text without spilling over.
* **parseHTML** _(Default: `'false'`)_ When true, parse and save html structure and restore structure in the truncated text.
* **onTruncate** _(Callback)_: Called after truncation is completed.
* **text** : text will be truncated. if not gave, element.html() will be truncated.
* **expendable** _(Default: false)_ When true, add expend link and collapse link at the end. you can customuze the two links by setting `more` and `less` config item.
* **resizeable** _(Default: true)_ When true, will retruncate text to fill current window size.
* **more** _(Default: 'more')_ text for expend link.
* **less** _(Default: 'less')_ text for collapes link. 

MIT License
-------
Copyright (c) 2016 Fuxian Ding (nekleding@gmail.com)

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
