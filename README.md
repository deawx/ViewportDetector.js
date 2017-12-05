<p align="center"><a href="https://projects.spope.fr/viewport/example/index.html" target="_blank"><img width="100" height="100" src="https://raw.githubusercontent.com/Spope/ViewportDetector.js/master/example/icon.png"></a></p>

# ViewportDetector.js

Javascript viewport element visibility library

ViewportDetector is a **lightweight** (1kb Gzipped) dependancy free library to detect if an element is in the viewport or not. It use **requestAnimationFrame** API to be without any impact on the performance.

## Installation

Just include the minified version of ViewportDetector.js on your website :


```html
<script src="viewportdetector/build/viewportdetector.min.js"></script>
```

## Usage

To use viewport detector, create a new instance :

```javascript
var detector = new ViewportDetector({
    selector: '.element',
    callback: myCallback
});
```
## Parameters

Here is the list of available parameters :

Name | Default value | Description
-----|---------------|------------
callback|Null|Callback to execute on visibility change. Callback receive **2 parameters**, the DOMElement and the Visibility (boolean).**Required**
selector|Null|Element selector. **Required**
opts|Null|Options. Currenlty only **marge** is avaliable.

## API

Here is the list of available APIs :

Name|Description
----|-----------
add(selector, callback, opts)|Add en element to detect into a instance of ViewportDetector

## Example

[See website](https://projects.spope.fr/layout/example/index.html)

## License

MIT

Made by [Spope](https://spope.fr/)