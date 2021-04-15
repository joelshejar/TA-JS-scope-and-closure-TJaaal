Create the execution context diagram for following code. What will be the output in each line of code

```js
function getCounter() {
  let privateCounter = 0;
  function changeBy(val) {
    privateCounter += val;
  }
  return {
    increment: function () {
      changeBy(1);
    },
    decrement: function () {
      changeBy(-1);
    },
    value: function () {
      return privateCounter;
    },
  };
};

let counter = getCounter()

counter.value();  // output 0
counter.increment(); // output 1
counter.increment(); // output 2
counter.value(); // output 2
counter.decrement(); // output 1
counter.value(); // output 1
```

2. Create the execution context diagram and write the output.

```js
function makeCounter() {
  let privateCounter = 0;
  function changeBy(val) {
    privateCounter += val;
  }
  return {
    increment: function() {
      changeBy(1);
    },

    decrement: function() {
      changeBy(-1);
    },

    value: function() {
      return privateCounter;
    }
  }
};

let counter1 = makeCounter();
let counter2 = makeCounter();

console.log(counter1.value());  // OUTPUT 0

counter1.increment();
counter1.increment();
console.log(counter1.value()); // OUTPUT 2

counter1.decrement();
console.log(counter1.value()); // OUTPUT 1
console.log(counter2.value()); // OUTPUT 1
```