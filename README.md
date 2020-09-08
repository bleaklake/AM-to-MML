# am-to-mml

This MathJax wrapper converts AsciiMath (AM) to Mathematical Markup Language (MML). This package doesn't use any webworkers, webviews ; so It can be used for your NodeJS, React and React Native projects.

**This project is still in its early development stages.**

For any bugs, typos, errors, feel free to open an issue on the associated Github repository.

## Installation

```cli
npm install am-to-mml --save
```

## Examples

### JS

```js
const AMToMML = require("am-to-mml");

const myAMEquation = "d/dxf(x)=lim_(h->0)(f(x+h)-f(x))/h";

const MMLEquation = AMToMML(myAMEquation); // returns <math xmlns="http://www.w3.org/1998/Math/MathML"><mstyle displaystyle="true"><mfrac><mi>d</mi> ...
```

### TS

```ts
import AMToMML from "am-to-mml";

const myAMEquation = "d/dxf(x)=lim_(h->0)(f(x+h)-f(x))/h";

const MMLEquation = AMToMML(myAMEquation); // returns <math xmlns="http://www.w3.org/1998/Math/MathML"><mstyle displaystyle="true"><mfrac><mi>d</mi> ...
```

## Documentation

`AMToCHTML(equation)` : **string** _The returned Mathematical Markup Language equation_

> `equation` : **string** _The AsciiMath equation_

## Notes

### Useful links

This wrapper is inspired by this project : https://github.com/mathjax/MathJax-demos-node/tree/master/direct.

### Typescript

You **DON'T** have to install any types `@types/am-to-mml`.
