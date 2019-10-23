# React JS Basics and Resources

React is a popular Javascript library used to build front-end user interfaces (UI). It uses component-driven-development to quickly build interfaces using reusable elements. It also streamlines how data is stored and handled using _state_ and _props_.

React is an open-source project developed and used by Facebook, with a large community of users developing with it and a lot of technology companies using it as part of their tech stack.

I've been working with React since 2018. This document is a working list of the things I've learned about React since then.

---

## Before You Start with React JS

You'll need to know some stuff, and you'll need to install some stuff on your machine.

### What knowledge you'll need before you start

There are some bases you'll likely want to cover before you start working with React:

- [Some experience in and understanding of web development, including HTML & CSS](https://www.khanacademy.org/computing/computer-programming/html-css) because React is used for web development
- [A solid understanding of Javascript concepts](https://developer.mozilla.org/en-US/docs/Web/JavaScript/A_re-introduction_to_JavaScript) because React is a Javascript library
- [Basic Command Line proficiency](https://www.taniarascia.com/how-to-use-the-command-line-for-apple-macos-and-linux/) because we'll be working with NPM on the command line (more about NPM below)
- [An understanding of the Document Object Model - the DOM](https://www.taniarascia.com/introduction-to-the-dom/) because React uses a Virtual DOM to re-render only the components that have changed, not the whole page

_~_~_~_~_~_~_~_~_~_

### What you need to install before you start

To run React locally, you'll need to be running Node and NPM on your machine.

[Node](https://nodejs.org/en/) - JavaScript is a client-side programming language, which means it’s processed in the browser. With the advent of Node.js, JavaScript can also be used as a server-side language.

[NPM](https://www.npmjs.com) - NPM, (which doesn't stand for Node Package Module) is the tool to connect to the repository containing all the Node.js programs, plugins, modules and so on.

For more information, read [How to Install and Use Node.js and npm (Mac, Windows, Linux)](https://www.taniarascia.com/how-to-install-and-use-node-js-and-npm-mac-and-windows/)

---

## Getting Started with React JS

There are a number of [toolchains](https://reactjs.org/docs/create-a-new-react-app.html#recommended-toolchains) you can use to start using React.

One of the simplest toolchains to use is [Create React App](https://create-react-app.dev/), which is a quick and easy way to start building a new [single-page application](https://reactjs.org/docs/create-a-new-react-app.html#recommended-toolchains) in React.

On a machine with NPM and Node installed, run the following commands using a Command Line Interface (I like working in Microsoft's [Visual Studio Code](https://code.visualstudio.com/) )

<pre><code>npx create-react-app my-app
cd my-app
npm start
</code></pre>

[# Full instructions & more configuration options for Create React App.](https://create-react-app.dev/docs/getting-started/)

_~_~_~_~_~_~_~_~_~_

Ok, so there's a few more things you might want to know - these aren't deal breakers, but will make your life easier when working with React.

- [Javascript XML](https://alligator.io/react/jsx-introduction/) (JSX) - language extension for writing the UI logic for your React components. JSX is meant to look a lot like HTML syntax, and is used to describe UIs, which React transforms into DOM elements. You are not required to use JSX, but JSX makes it easier to write React applications.
- [TypeScript](https://www.typescriptlang.org/) (tsx) - TypeScript is JavaScript for application-scale development. TypeScript is a strongly typed, object oriented, compiled language. It is predictable, is self-documenting in some aspects, and generally easy to debug.
- [Sassy CSS](https://sass-lang.com/) (scss) - SCSS is a CSS preprocessor which allows you to use features like variables, mixins and nested rules in CSS, which makes life so much easier, and makes code easier to maintain.

---

## Fundamentals of React JS

### Component-driven development

> "Component-Driven Development (CDD) is a development methodology that anchors the build process around components. It is a process that builds UIs from the “bottom up” by starting at the level of components and ending at the level of pages or screens."
>
> https://blog.hichroma.com/component-driven-development-ce1109d56c8e#.ltre4c82b

Components let you split the UI into independent, reusable pieces, and think about each piece in isolation. Think about React components like functions that return HTML elements (via a render function).

A component might be something like a button, a modal, or a date picker. Components are often nested, and may have many parents/ ancestors, and children/ decendents. Like Russian Dolls. For example, a modal component may have a nested header component, which may have it's own nested title component.

React has two types of components: Class Components and Function Components.

The raw data that the HTML output derives comes from _state_ and _props_. Changes to the props and state trigger a render update to the Virtual Dom. State and Props can alter the attributes of a component.

[# A huge list of resources about component driven development](https://github.com/component-driven/awesome-list)

#### Props

Props is short for "properties". Props are plain JavaScript objects that hold information which influences the output f the render. Props are passed into a component from its parents and are immutable. A component cannot change its own props, but it is responsible for passing down props to it's own child components.

#### State

When a component 'mounts' (renders for the first time), it will have a default 'state'. Through events (usually generated by the user), the state will change. State is mutable. Components manage their own states, but do not mess with the state of their children (beyond setting a default value)

Beyond the interface, you'll need something to deal with state. Here are some options...

---

## Going Further with React JS

One way to do it is with Redux. Redux deals with state management

- Actions
- Reducers
- Store

What can redux do?

- Manipulate the state
- Receive the state
- Listen to the state changes

Read More - [Reasons to learn Redux as a JavaScript Developer](https://www.robinwieruch.de/redux-javascript)

---

### React Filing Systems

Dan Abramov famously said, ["move files around until it feels right"](https://react-file-structure.surge.sh)

---

### Further Reading - Various Links in no particular order

- [Thinking in React](https://reactjs.org/docs/thinking-in-react.html)
- [JavaScript fundamentals to master before learning React](https://www.robinwieruch.de/javascript-fundamentals-react-requirements)
- [Complete Intro to React V5](https://btholt.github.io/complete-intro-to-react-v5/)
- [8 things to learn in React before using Redux](https://www.robinwieruch.de/learn-react-before-using-redux)
- [What is a reducer (React/Redux) in JavaScript?](https://www.robinwieruch.de/javascript-reducer)
- [React Redux Tutorial for Beginners 2019](https://www.robinwieruch.de/react-redux-tutorial)
- [Idiomatic Redux: The History and Implementation of React-Redux](https://blog.isquaredsoftware.com/2018/11/react-redux-history-implementation/)
- [React Toolchains](https://reactjs.org/docs/create-a-new-react-app.html)
- [Detailed API reference for the React component class definition](https://reactjs.org/docs/react-component.html)
- [React component lifecycle methods diagram](http://projects.wojtekmaj.pl/react-lifecycle-methods-diagram/)
- [More Javascript tutorials](https://www.digitalocean.com/community/tutorial_series/how-to-code-in-javascript)
- [React Glossary of Terms](https://reactjs.org/docs/glossary.html)
- [Getting started with React](https://www.taniarascia.com/getting-started-with-react/)
- [Create React App docs](https://create-react-app.dev/docs/getting-started)
- [Create React App on Github](https://github.com/facebook/create-react-app#creating-an-app)
- [Design Systems for Developers](https://www.learnstorybook.com/design-systems-for-developers/react/en/introduction/)
- [Should you learn React? Check out this Software Developer Roadmap](https://github.com/kamranahmedse/developer-roadmap)

##### Bundlers

Bundling is the process of combining and optimizing multiple modules into one or more production ready bundles, mostly concenred with making code ready for production

- Webpack - https://webpack.js.org/
- Rollup - https://rollupjs.org/guide/en
- Google Closure Compiler - https://github.com/google/closure-compiler/wiki
- Parcel - https://parceljs.org/
- Browserify - http://browserify.org/
- FuseBox - https://fuse-box.org/

https://medium.com/@ajmeyghani/javascript-bundlers-a-comparison-e63f01f2a364

---

# Checklist

Understand the Basics

- [ ] Web development
- [ ] Javascript
- [ ] Document Object Model (DOM)
- [ ] Basic command line proficiency

Install on your machine

- [ ] Node JS
- [ ] NPM

Create a React Application

- [ ] Create a new app with Create React App

Get your head around these 'quality of life' langauges for React

- [ ] JSX
- [ ] TSX
- [ ] SCSS

Component driven development

- [ ] Understand 'state'
- [ ] Understand 'props'
