# High Resolution Timer

[`performance.now()`](https://developers.google.com/web/updates/2012/08/When-milliseconds-are-not-enough-performance-now) returns the number of milliseconds (floating point num) since the beginning of the page load. In contrast to `Date.now()` it doesn't depend on system time and the clock time shift.
