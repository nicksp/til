# 100vh in Safari iOS

In Safari on iOS an element with the height of `100vh` can have different height depending on the way Safari calculated viewport height: with 'minimal' or 'full' toolbar.

The funny thing — [this isn't a bug, it's a feature](https://nicolas-hoizey.com/2015/02/viewport-height-is-taller-than-the-visible-part-of-the-document-in-some-mobile-browsers.html).

> This is completely intentional. It took quite a bit of work on our part to achieve this effect.
