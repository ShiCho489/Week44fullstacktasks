# Homework

We try to go through the following exercises tomorrow (in the first group discussion). Please make sure that you are prepared before class.  

## Exercise 1
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
Answer-5
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
```Answer- 12

3. 

```js
const ages = [3, 10, 18, 20];

function checkAge(age) {
  return age > 18;
}

console.log(ages.find(checkAge)); 
```answer-20

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

## Exercise 2

- How this code works? Pay attention to `Number()`.
```js
const d = new Date("December 17, 1995 03:24:00");
console.log(Number(d));
```

## Exercise 3
- What is the relationship between CRUD operations and HTTP methods?
 The primary or most-commonly-used HTTP verbs (or methods, as they are properly called) are POST, GET, PUT, PATCH, and DELETE. These correspond to create, read, update, and delete (or CRUD) operations, respectively. There are a number of other verbs, too, but are utilized less frequently.
- What is the difference between `routes` and `endpoints`?
Endpoints perform a specific function, taking some number of parameters and return data to the client. A route is the “name” you use to access endpoints, used in the URL. A route can have multiple endpoints associated with it, and which is used depends on the HTTP verb.
- Discuss the following HTTP response status codes: `200, 204, 403, 404`.¨
200-ok
204-No content
403-forbidden
404-not found

## Links
- [find()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/find)
- [Number()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)
- [HTTP response status codes](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status)
- [CRUD](https://en.wikipedia.org/wiki/Create,_read,_update_and_delete)