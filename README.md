# React-Mastery
Master React With This Notes
# 🚀 React Notes

## 📖 Table of Contents
- [How does React’s Virtual DOM work?]
- [React Basics](#react-basics)
- [Components](#components)

---

## 📌 Introduction
React is a JavaScript library for building user interfaces. It allows developers to create reusable UI components and manage state efficiently.

## ⚛️ 1. How does React’s Virtual DOM work?
- React’s Virtual DOM is a lightweight copy of the actual DOM. When state changes, React first updates the Virtual DOM instead of changing the real DOM directly. It then compares the new Virtual DOM with the previous one, finds the differences (diffing), and updates only the changed parts in the real DOM (reconciliation). This makes React fast.

## ⚛️ 1. What is npm?
- npm is default package manager for Node.js, it allows developers to install, share, manage packages or modules and dependencies for their project.

## ⚛️ 1. What is package.json?
- Package.json file is a configuration for npm.

## ⚛️ 1. What is package-lock.json?
- Package-lock.json file maintains exact version of packages.

## ⚛️ 1. What is Node module?
- Node module is a collection of dependencies

## ⚛️ 1. Why react apps are fast?
- 🚀 React fiber(the new reconcilation alogorithm) which finds out the diffrence between two virtual dom's (new virtual DOM and Old Virtual DOM) and updates only the portion is required. thats is the main reason of Why react is fast.

## ⚛️ 1. What is Babel?
- Babel is a javaScript compiler or transpiler which is used to convert React.Elements into HTML like structure.

## ⚛️ 1. What is component?
- Component is a normal javaScript functions which returns a small piece of JSX.

## ⚛️ 1. How JSX works behind the scene?
- JSX => React.createElement => (convert to) ReactElement js Object => (then render as a) HTML Element.
- Babel is responsible to convert jsx and render that HTML Element.
- Babel takes this jsx code 

let heading = <h1 class="yash">Hello Babel</h1>

and convert it into this code 
```jsx
let heading = React.createElement("h1", {
  class: "yash"
}, "Hello Babel");
```
## ⚛️ 1. What is Congigue Driven UI
- JSX => in your header section there is crousel and in diffrent state you want to show new offers.
- ex. in Maharastra you want to show 50% offer and in Delhi you want to show 40% offers then you dont create diffrent applications for diffrent states. there you need you use concept is (Configue Driven UI).

## ⚛️ 1. How does useEffect Works?
- Syntax
- ```jsx useEffect(()=>{}, []) ```
- 1. Every time a component render then useEffect will be called.
  2. if there is no dependency array => useEffect is called in every render.
  3. if dependency array is empty = [] => useEffect is called on initial render(just onece)
  4. if dependency array is [btnNameReact] => called everytime btnNameReact is updated.

