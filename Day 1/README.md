# _How does JavaScript work?_

To get to that, first let's have some basics right.

Note : you don't need to master these, we're going to explore these in detail later.

Just knowing what they mean is enough ☺

---
### What is asynchronous in JavaScript?

_Understanding Asynchronous JavaScript_ - https://youtu.be/_IGIQ10yX1o

---
### What is a callback? 
(We have detailed lecture for this, don't worry too much about it)

_Understanding JavaScript Callbacks_ - https://youtu.be/Nau-iEEgEoM


If you already know what they are you can skip these videos.

But I want you to know that *__setTimeOut__* is asynchronous and accepts a callback.

---

### So how does JavaScript engine work?

_Andrei Neagoie_ - https://youtu.be/hGSHfObcVf4

---

#### Exercise

Guess the output of the following and the reason why you recieve the output that you do?

```
console.log('1');
setTimeout(() => {
        console.log('2')
},0);

console.log('3');
```

Note : PFA the notes for this topic and try to read them twice (before and after watching the video)
