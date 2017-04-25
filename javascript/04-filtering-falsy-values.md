# Filtering falsy values

Quickly discard falsy values from an Array using filter(Boolean). This is like `lodash.compact`.

```js
> ['this', 'has', undefined, false, 0, null, NaN, 'values'].filter(Boolean)
[ 'this', 'has', 'values' ]
```

This works because Boolean(val) is roughly equivalent to val => !!val. That is, it’s a function that coerces a value into a Boolean.
