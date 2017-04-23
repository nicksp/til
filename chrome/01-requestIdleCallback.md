# requestIdleCallback

As of Chrome version 47 there's a companion tool for `requestAnimationFrame` available — `requestIdleCallback` function. The browser will invoke the passed callback when there is free time at the end of a frame, or when the user is inactive. How and when to use it can be discovered at [Google Developers](https://developers.google.com/web/updates/2015/08/using-requestidlecallback).

In browsers other than Chrome, use shims from below:

* [https://gist.github.com/paullewis/55efe5d6f05434a96c36](https://gist.github.com/paullewis/55efe5d6f05434a96c36);
* [https://github.com/aFarkas/requestIdleCallback](https://github.com/aFarkas/requestIdleCallback).
