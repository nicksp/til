# console.time()

`console.time` and `console.timeEnd` measure and display time spent executing code in milliseconds:

```js
let i, output = '';

// Start timing now
console.time('calculateConcatenation');

for (i = 1; i <= 1e6; i++)
    output += i;

// ... and stop
console.timeEnd('calculateConcatenation');
```

![console time](/_assets/console-time-example.png)
