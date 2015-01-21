# Iterators Lab

### Description

In the iterators lab we will be continuing our exploration of
iterators. We have a series of challenges that require you to use the
iterators we discussed in class. We will try to use various testing
methods to verify that your code is working.

### Phase-1

Research the following term and summarize your findings on it two to
three sentences:

* `higher-order function`


Update this README with a description of each of the following and an
example you've created:

* `forEach`: forEach retrieves each element from an array and performs a function upon it. It operates in ascending order, and can take arguments for the callback function it will be performing. The syntax looks as thus: array.forEach(callback, (argument)).
* `map`: map creates a new array populated with the result of performing a function on each element of the source array. map performs this in ascending order, and populates the new array accordingly. 
* `filter`: filter creates a new array that is populated with elements of the source array that pass a test. A callback function is placed in the syntax that, when it returns true, populates a new array. If false, the element is left out of the new array. 
* `reduce`: the reduce function performs some function upon the array, in ascending order, that combines two elements in some way. Eventually, through this cascading effect, the reduce method will return a single value. The parameters for the combining function default to the first and second elements of the array. 
* `some`: some is a method that applies a test function to each element of an array until it returns true. Unlike filter, which does something comparable but then populates a new array, some searches through until an element makes the function true, then simply returns true. If no element satisfies the function, some returns false. 
* `every`: every is like the opposite to some. every searches through an array, testing each element against a function. It does this for every element until one returns a falsey value, at which point every returns false. If all elements of the array satisfy the every callback function, every returns true. 
Use the notes provided to help guide you explanation.

### Phase-2

* Run `npm install` from the `iterators_lab` directory.
* Looks at the tests we've written in the `test` folder. Run the tests
  with `npm test` (also from the `iterators_lab` directory). They
  should all fail.
* Get all of the tests to pass by writing the necessary code in
  `src/iterators.js`.

### Phase-3

Refactor the following code using `map` to make only one call to the `map` function versus the two below.


```
var myNumbers = [ -1, 2, -3, 4, -5, 6];

var square = function(num) {
	return num * num;
};

var sqrRoot = function(num) {
	return Math.sqrt(num);
};


var sqrNumbers = map(myNumbers, square);
var absNumbers = map(sqrNumbers, sqrRoot);
```




