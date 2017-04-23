# Quick tap in Safari

In Safari on iOS they're [eliminating 350ms tap delay](https://webkit.org/blog/5610/more-responsive-tapping-on-ios/). Responsive tapping is enabled under the following conditions:

* unscalable viewports (`user-scalable=no` or a `minimum-scale` equals to the `maximum-scale`);
* `width=device-width`  when the user is at initial scale;
* putting `touch-action: manipulation` on an elements styles.
