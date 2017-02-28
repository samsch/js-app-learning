Before trying to learn React or Redux, or use Webpack/Browserify or Babel, you should make sure you know Javascript at least reasonably well. A great resource learning Javascript is [EloquentJS](http://eloquentjavascript.net/). If you have never programmed before, another great place to learn JS is [Codecademy](https://www.codecademy.com/). The best resource for referencing the basic web languages (HTML, CSS, Javascript, and the DOM API) is the Mozilla Developer Network, commonly referred to as [MDN](https://developer.mozilla.org/).

# Basic setup

- [create-react-app](https://github.com/facebookincubator/create-react-app)
 - This is a relatively new tool from facebook, which gets you up and running with a good development environment (Webpack+Babel+ESLint) quickly. It also includes an escape for when you need to use custom configuration.
- [Setting Up a React.js Environment Using Npm, Babel 6 and Webpack](https://www.codementor.io/reactjs/tutorial/beginner-guide-setup-reactjs-environment-npm-babel-6-webpack)
 - It's potentially hazardous to use ES2015 import/export syntax, as the loading definition is non-existant. Right now Babel compiles it to CommonJS, and it's better to use that directly.
- A quickly runnable final config/boilerplate React app (based on the above Codementor tutorial) is available here: https://github.com/samsch/basic-react.
 - This repo also includes the bit of webpack configuration which puts React into production mode for the production build, which is missed in the Codementor tutorial.

# React

- [React Docs](https://facebook.github.io/react/docs/getting-started.html)
 - Remember that the most basic guides makes generalizations and simplifications such that they aren't great references for "good" coding. The *Guides*, *References*, and *Tips* sections are your good references.
- [React.js Introduction For People Who Know Just Enough jQuery To Get By](http://reactfordesigners.com/labs/reactjs-introduction-for-people-who-know-just-enough-jquery-to-get-by/)
- [React Training](https://github.com/ryanflorence/react-training)
  - [Wrapping DOM Libs](https://github.com/ryanflorence/react-training/blob/gh-pages/lessons/05-wrapping-dom-libs.md)

- [Learn about immutability](http://reactkungfu.com/2015/08/pros-and-cons-of-using-immutability-with-react-js/)
- [Basic immutable state with PureComponent example](http://codepen.io/anon/pen/ryOvwG?editors=0011)

### Tips
- The best way to use React is to stick (almost) exclusively to passing down props (for state and callbacks), and ignoring component state. You should almost always be able to use [stateless function components](https://facebook.github.io/react/docs/reusable-components.html#stateless-functions).

### Getting help
Google and the React docs should be your first place to go for React help. If you can't find your answer there, check out the #reactjs IRC channel on Freenode, or the [Reactiflux Discord](http://www.reactiflux.com/) channel.

# Redux

Redux is a flux-like application state store. Redux (and indeed, any framework or flux implementation) is not needed to build good Javascript applications. That said, if you want a set structure for how to build you app (a framework), Redux is a good choice. Another popular choice is [Alt](http://alt.js.org/), which is supposed to have very good docs for learning Flux.

Most Redux docs and tutorials assume you know some of the most commonly used ES2015 syntax; notably arrow functions, destructuring, and import syntax.

> One thing that many are getting wrong is using import syntax, and having Babel compile it to CommonJS. **Do not use ES2015 import syntax.** It's behavior is **currently undefined!**. You can see where it's at [here](https://github.com/whatwg/loader). Instead, use CommonJS directly.
> -- My opinion

### Basics

- [Redux creator's intro videos](https://egghead.io/series/getting-started-with-redux)
- [Redux Docs](http://redux.js.org/)

1. The best way to get started with the Redux docs is to read (and code along with) section 1 through 1.3, skip 1.4 and 1.5 for now, and then go through sections 2 and 3.
2. Section 2.5 requires you have a bit of an idea how React components work, specifically [stateless function components](https://facebook.github.io/react/docs/reusable-components.html#stateless-functions), combined with arrow functions and destructuring.
3. Once you have gone through these basics, and gotten a small test app to work, try using what you know now to build a small app. Don't worry about "best practice" yet. Much of the best practice subjects don't make much sense until you actually try to do the things which it protects against.
4. Once you have built some small app with what you know, you might jump into the **Intermediate guides** below.

- [Redux FAQ (in the documentation)](http://redux.js.org/docs/FAQ.html)
- [High Level Description of Redux](http://www.youhavetolearncomputers.com/blog/2015/9/15/a-conceptual-overview-of-redux-or-how-i-fell-in-love-with-a-javascript-state-container)
- [Rules For Structuring (Redux) Applications](http://jaysoo.ca/2016/02/28/organizing-redux-application/)

### Intermediate guides

- [Presentational and Container Components](https://medium.com/@dan_abramov/smart-and-dumb-components-7ca2f9a7c7d0#.g1je0fegu)
- [Redux best practices](https://medium.com/lexical-labs-engineering/redux-best-practices-64d59775802e#.2ikgk77qm)

### Next steps

- [Using Elm architecture in Redux](https://github.com/reactjs/react-redux/issues/278#issuecomment-179137918)
- [Encapsulation in Redux](http://blog.javascripting.com/2016/02/02/encapsulation-in-redux/)

### Individual systems

- [Ducks: Redux Reducer Bundles](https://github.com/erikras/ducks-modular-redux)

### Getting help
Google and the Redux docs should be your first place to go for Redux help. If you can't find your answer there, check out the #reactjs IRC channel on Freenode (there isn't an active, Redux specific channel), or the [Reactiflux Discord](http://www.reactiflux.com/) Redux channel.
