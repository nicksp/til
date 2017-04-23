# initial in CSS

I often get confused with the default values for such properties as `max-height` (`none` instead of `auto`), `min-height` (`0` instead of `auto`) and `z-index` (`auto`, but not `0` or `none`). Fortunately for fellow forgetful developers like me, all modern browsers (except IE) can do `initial` keyword:

```css
max-height: initial; /* == none */
min-height: initial; /* == 0 */
z-index: initial; /* == auto */
```

IN more details [in spec](https://www.w3.org/TR/css-values/#common-keywords) and on [caniuse.com](http://caniuse.com/#feat=css-initial-value).
