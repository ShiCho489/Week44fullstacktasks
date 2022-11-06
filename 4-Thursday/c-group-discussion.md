
# Group Discussion

## Exercise 1
- Please follow the steps in the following [link](https://github.com/appacademy/practice-for-week-10-intro-to-express/blob/main/README.md)

## Exercise 2
- How these code snippets work? Pay attention to `find()`.

1. 

```js
const inventory = [
  { name: "apples", quantity: 2 },
  { name: "bananas", quantity: 0 },
  { name: "cherries", quantity: 5 },
];

function isCherries(fruit) {
  return fruit.name === "cherries";
}
console.log(inventory.find(isCherries));
```

2. 

```js
const array1 = [5, 12, 8, 130, 44];
const found = array1.find(element => element > 10);
console.log(found);
```
```js
const array1 = [5, 12, 8, 130, 44];
const found = array1.find(element => element > 10);
console.log(found);
```

3. 

```js
const ages = [3, 10, 18, 20];

function checkAge(age) {
  return age > 18;
}

console.log(ages.find(checkAge)); 
```

4. 

```js
function isPrime(element, index, array) {
  let start = 2;
  while (start <= Math.sqrt(element)) {
    if (element % start++ < 1) {
      return false;
    }
  }
  return element > 1;
}

console.log([4, 6, 8, 12].find(isPrime)); // undefined, not found
console.log([4, 5, 8, 12].find(isPrime)); // 5
```

## Exercise 3

- How this code works? Pay attention to `Number()`.
```js
const d = new Date("December 17, 1995 03:24:00");
console.log(Number(d));
```

## Exercise 4
- What is the relationship between CRUD operations and HTTP methods?
- What is the difference between `routes` and `endpoints`?
- Discuss the following HTTP response status codes: `200, 204, 403, 404`.

## Links
- [find()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/find)
- [Number()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)
- [HTTP response status codes](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status)
- [CRUD](https://en.wikipedia.org/wiki/Create,_read,_update_and_delete)
