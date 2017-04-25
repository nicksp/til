# @extend sucks

Using `@extend` in CSS preprocessors like Sass really suck… so use mixins instead.

Consider this example:

```css
%antialias {
  text-rendering: optimizeLegibility !important;
  -webkit-font-smoothing: antialiased !important;
  -moz-osx-font-smoothing: grayscale;
}
```

Seems harmless enough:

```css
h1 {
  @extend %antialias;
}
```

Until you try it with media queries:

```css
// You may not @extend an outer selector from within @media.
@media (max-width: 300px) {
  h3 {
    @extend %antialias;
  }
}
```

It won't work. You may not @extend an outer selector from within @media.
You may only @extend selectors within the same directive. Thus, use mixins instead.
