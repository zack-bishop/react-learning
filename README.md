# I. Introduction
- Video creator acknowledges that React is complicated thing
- Warning: Exercises that will be challenging
- I like that the author points out that failure is a better teacher than success
## Community
- Ugh.  They have a discord.
## Course Features
- Uses `Code Playgrounds`, i.e. Code Pens.
  - This is an interesting approach, as it might solve some of the typical issues people have setting things up
  - But, not sure if I like it, as I won't have the code on my personal machine / in this repo
- Kind of cool it has a built in note taking tool.
  - Might be especially useful if we had a Kanopi-account.
## Reference Modules
- There are two modules that discuss a lot of the "scaffolding" that one might need to take this course:
  - __JavaScript Primer__: I could definitely use this.
    - Here's an amazing [resource](https://courses.joshwcomeau.com/joy-of-react/00-introduction/03-course-features?peek=%2Fjoy-of-react%2F10-javascript-primer%2F04-arrow-functions) on using function short hand.
  - __Tools of the Trade__: is about using tooling one may need to get the most out of react.

# II. Module 1: React Fundamentals
## The Magic of React
- Built by Facebook.
- Book recommendation: [Rethinking Web App Development at Facebook](https://youtu.be/nYkdrAPrdcw?t=624)
- Sounds like state management is a big part of react.

## Hello React

```
import React from 'react'; // Import react
import { createRoot } from 'react-dom/client'; // platform-specific renderers.  This one is mainly used for the web.
```

- Apparently react does a lot of differ things
  - For example: `react-three-fiber` for 3D scenes using WebGL and Three.js
- Great explanation of what the `DOM` actually is:

```
**What the heck is the “DOM”, anyway?**

The DOM is the living, breathing structure that makes up a live website / web application. When we visit a website, the browser turns the static HTML into the DOM.

To use an analogy: HTML is the blueprint for a specific car, and the DOM is the car itself, zipping around the city.
```
- Creating an element is pretty self-explanatory.
- `document.querySelector` start using this instead of `document.getElementById`
- The `createRoot` function in `const root = createRoot(container)` function is what tells react what the base of the application is.
- `root.render(element)` is what actually converts the JavaScript element we created into an actual DOM element
- The following is outdated:

```
import ReactDOM from 'react-dom';

ReactDOM.render(
  element,
  container
);
```
### Video: Build Systems
- react is __always__ used as part of a build system.
- The code playgrounds have built in build systems.
- I don't like how the code is in these Code Pens.  I'd prefer it to have the files running locally.
- React uses `JSX`
- Learn more about this in the [“Tools of the Trade” reference module](https://courses.joshwcomeau.com/joy-of-react/11-tools-of-the-trade)

## Exercise: Build Your Own React
- This exercise has us "rebuild" some things that React does using vanilla javascript.
- THe idea is to de-mystify what it's doing.
- Basically, React creates a "virtual DOM" of elements that get written into the actual DOM.
- Great quote about `Productive Failure`:

```
In Productive Failure, the conventional instruction process is reversed so that learners attempt to solve challenging problems ahead of receiving explicit instruction. While students often fail to produce satisfactory solutions (hence “Failure”), these attempts help learners encode key features and learn better from subsequent instruction (hence “Productive”).
```
- Need to have a `Growth Mindset`.
- 
# Reference Module: JavaScript Primer:
- Has an excellent article on functional short hand, aka: `Arrow Functions`
