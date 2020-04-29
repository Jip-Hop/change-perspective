# css3-perspective

A very small JavaScript library (no dependencies!) for creating CSS3 perspective transforms.

Based on [change-perspective](https://github.com/Volst/change-perspective).

## Install

```
Copy index.js where you need it (rename if you like).
```

## Usage

```js
import fixPerspective from "index.js";

const srcCorners = [158, 64, 494, 69, 495, 404, 158, 404];
const dstCorners = [100, 500, 152, 564, 148, 604, 100, 560];

const H = fixPerspective(srcCorners, dstCorners);
const t = "matrix3d(" + H.join(", ") + ")";
document.querySelector("div").style.transform = t;
```
