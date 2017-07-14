# Pretty printing JSON

Have you ever had the need to print out a JSON structure for debugging? Something like:

```js
console.log(`the data is ${JSON.stringify(data)}`);
```

And then the result is a unformatted JSON structure that you copy/paste into your editor for prettyprinting? Well there is a way to avoid that last step. Just pass in two more magic arguments to `JSON.stringify` and you get prettyprinted JSON right out of the box.

```js
console.log(`the data is ${JSON.stringify(data, null, 2)}`);
```
