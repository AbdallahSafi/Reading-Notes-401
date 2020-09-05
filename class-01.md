# Node Ecosystem, TDD, CI/CD

## JavaScript Array map() Method

- The map() method creates a new array with the results of calling a function for every array element.

- The map() method calls the provided function once for each element in an array, in order.

- map() does not execute the function for array elements without values.

-  this method does not change the original array.

### Syntax

`array.map(function(currentValue, index, arr), thisValue)`


## JavaScript Array reduce() Method

- The reduce() method reduces the array to a single value.

- The reduce() method executes a provided function for each value of the array (from left-to-right).

- The return value of the function is stored in an accumulator (result/total).

- reduce() does not execute the function for array elements without values.

- this method does not change the original array.

### Syntax

`array.reduce(function(total, currentValue, currentIndex, arr), initialValue)`

## Superagent

### With normal Promise .then() syntax

```javascript
function getData(){
 superagent.get(url).then(res =>{
    console.log(res)
})
}
```

###  with async / await syntax

```javascript
async function getData(){
    let data = await superagent.get(url);
    console.log(data);
}
```

## JavaScript Promises

A Promise in short:

"Imagine you are a kid. Your mom promises you that she'll get you a new phone next week."

You don't know if you will get that phone until next week. Your mom can either really buy you a brand new phone, or she doesn't, because she is not happy :(.

That is a promise. A promise has 3 states. They are:

1. Pending: You don't know if you will get that phone
2. Fulfilled: Mom is happy, she buys you a brand new phone
3. Rejected: Mom is unhappy, she doesn't buy you a phone

```javascript
var isMomHappy = false;

// Promise
var willIGetNewPhone = new Promise(
    function (resolve, reject) {
        if (isMomHappy) {
            var phone = {
                brand: 'Samsung',
                color: 'black'
            };
            resolve(phone); // fulfilled
        } else {
            var reason = new Error('mom is not happy');
            reject(reason); // reject
        }

    }
);

var willIGetNewPhone = ... // continue from part 1

// call our promise
var askMom = function () {
    willIGetNewPhone
        .then(function (fulfilled) {
            // yay, you got a new phone
            console.log(fulfilled);
             // output: { brand: 'Samsung', color: 'black' }
        })
        .catch(function (error) {
            // oops, mom don't buy it
            console.log(error.message);
             // output: 'mom is not happy'
        });
};

askMom();
```


## Are all callback functions considered to be Asynchronous? Why or Why Not?

### Argument function can be called synchronously

Simply taking a callback doesn't make a function asynchronous. There are many examples of functions that take a function argument but are not asynchronous. For example there's forEach in Array. It iterates over each item and calls the function once per item.

```javascript
  var totalSize = 0;
    items.forEach((item) => {
        totalSize += item.size;
    });
    return totalSize;

```

### Asynchronous function needs to perform an asynchronous operation

For a function to be asynchronous it needs to perform an asynchronous operation. It needs to incorporate the argument callback in handling the results of this asynchronous operation. Only this way the function becomes asynchronous.

For example a function reading contents of a file with the correct encoding can be implemented as an asynchronous function.

```javascript
function readFileAsUtf8(filename, callback)
    fs.readFile(filename, "utf8", function(err, data) =>  {
        callback(data);
    });
}
```
