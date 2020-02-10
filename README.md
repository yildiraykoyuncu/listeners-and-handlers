# Listeners & Handlers

This repository contains a some mini-websites for you to study and practice developing.  Each one has some HTML a few listeners and handlers with blanks to fill in, and each one is organized the same way. The goal of these exercises isn't to create mind-blowing projects. Instead the goal to get lots of practice reading code, debugging and stepping through in the debugging.

* [How to do the exercises](#how-to-do-the-exercises)
* [The exercises](#the-exercises)

> You should already know a little about events before getting working on these exercises, head over to [study.hackyourfuture.be](https://study.hackyourfuture.be/javascript/events) to find some starting resources

---

## How to do the exercises

To complete the exercises you should copy-paste the code from `challenge.html` into the file `solution.html`, this will help you go back to the beginning when you make mistakes and to review what you learned later.

Each `challenge.html` contains multiple blanks (`_`) to fill in.  Your task is to replace each one with the correct word.  All of the words you need to fill in the blanks are already somewhere in the challenge, you just need to find them!

For example in the first exercise:

```html
<head>
  <script id='handlers'>
    function handler(event) {
      debugger;
      console.assert(event.target.innerHTML === '_', 'event.target.innerHTML');
      console.assert(event.target.nodeName === '_', 'event.target.nodeName');
      console.assert(event.target.id === 'hi', 'event.target.id');
      console.assert(event.target.className === 'secret', 'event.target._');
      console.assert(event.type === 'click', 'event.type');
    }
  </script>
</head>
<body>
  <section id='user-interface'>
    <button id='hi' class='secret'>catch me if you can!</button>
  </section>

  <script id='listeners'>
    document.getElementById('_').addEventListener('_', _);
  </script>
</body>
```

The best way to solve the exercises is to start by studying the code in `<script id='handlers'>`, and working "backwards" from there.  This will help you know what you are looking for in the rest of the file, for example in the code above:

* `event.type === 'click'` shows that you should be adding a "click" event, so you can fill in the event type like this: `document.getElementById('_').addEventListener('click', _);`
* `event.target` is the HTML element that the event is attached to.  So when you see `event.target.id === 'hi'` in the handler, you can fill in the event listener like this: `document.getElementById('hi').addEventListener('click', _);`

An enormous part of programming is actually just reading! Spotting relationships between lines of code, or finding small changes or mistakes in a file of code is a crucial skill to develop.

To get an idea of how this works, it will be very helpful to start by studying [the completed example](./z-example).  Open both the example `challenge.html` and the example `solution.html` in Visual Studio Code and compare them side-by-side, can you find find how each blank was filled in?

---

## The Exercises

* [Completed Example](./z-example)
* [Exercise 1](./exercise-1)
* [Exercise 2](./exercise-2)
* [Exercise 3](./exercise-3)

---
---

### <a href="https://hackyourfuture.be" target="_blank"><img src="https://user-images.githubusercontent.com/18554853/63941625-4c7c3d00-ca6c-11e9-9a76-8d5e3632fe70.jpg" width="100" height="100" alt="Hack Your Future: Belgium"></a>
