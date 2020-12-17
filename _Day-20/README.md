# _JavaScript interview questions_

Here is a list of JavaScript interview questions I collected from various resources and asked around.

---
##### Links:

- [37 Essential JavaScript Interview Questions](https://www.toptal.com/javascript/interview-questions)

---
##### Q. What are the two important  programming paradigms?
 _Answer:_ OOP and functional programming

---

##### Q. What is functional programming?
 _Answer:_ 
        - Pure functions / function purity.
		- Avoid side-effects.
		- Simple function composition.
		- Mention of features that support FP: first-class functions, higher order functions, functions as arguments/values.

---

##### Q. What is asynchronous programming, and why is it important in JavaScript?

---

##### Q. Explain about how user will be blocked if no asynchronous programming and how it works in JavaScript (day 1 notes) and new job queue after promises came into picture.

---

##### Q. What is an IIFE? How can it be useful (explain about how we can avoid overriding global variables)

---

##### Q. Difference between == and ===

---

##### Q. Output of following:

```JavaScript

var myObject = {
    foo: "bar",
    func: function() {
        var self = this;
        console.log("outer func:  this.foo = " + this.foo);
        console.log("outer func:  self.foo = " + self.foo);
        (function() {
            console.log("inner func:  this.foo = " + this.foo);
            console.log("inner func:  self.foo = " + self.foo);
        }());
    }
};
myObject.func();
```

Answer :
```JavaScript

outer func:  this.foo = bar
outer func:  self.foo = bar
inner func:  this.foo = undefined
inner func:  self.foo = bar
```
---

##### Q. Why was block scope introduced? Why should we use let and const instead of var?

---

##### Q. What are the benefits of using ‘use strict' in JavaScript?

---

##### Q. Output of following:

```JavaScript

(function() {
    console.log(1);
    setTimeout(function(){console.log(2)}, 1000);
    setTimeout(function(){console.log(3)}, 0);
    console.log(4);
    })();
```
---

##### Q. Output of following:

```JavaScript
for (var i = 0; i < 5; i++) {
	setTimeout(function() { console.log(i); }, i  );
}

How are you going to fix it?

Hint: Use let instead of var (let has block scope so value is different for every iteration)
```

---

##### Q. What is the output out of the following code? Explain your answer.

```JavaScript

var a = {},
    b = {key:'b'},
    c = {key:'c'};

a[b] = 123;
a[c] = 456;

console.log(a[b]);
```

Answer: https://www.toptal.com/javascript/interview-questions

---

##### Q. How are you going to do error handling with promises?

---

##### Q. What are the types of array and functions is JavaScript? (Objects)?

---

##### Q. What is argument objects in JavaScript & what  type of arguments passed to a function?

---

##### Q. What is a callback?

---

##### Q. What is difference between call, apply and bind?

---

##### Q. Write a sum method which will work properly when invoked using either syntax below:

```JavaScript

console.log(sum(2,3));   // Outputs 5
console.log(sum(2)(3));  // Outputs 5
```

Hint: Use currying to do it.

---

