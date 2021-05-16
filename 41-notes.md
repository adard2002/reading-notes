# Reading 41 Notes

[Home](README.md)

# React Native

## Vocab Terms
### redux toolkit slices: https://www.softkraft.co/how-to-setup-slices-with-redux-toolkit/
1. What is create slice?
This is a function that deals with everything you need for every slice. This is the most valuable of using Toolkit.
2. Returned object from createSlice contain:
- name: parameter which will be the prefix for all of your action types
- initialState: initial values for our reducer
- reducers: is an object where keys will become action type strings and the functions will be reducers that will be run when that action type is dispatched
3. Adding actions

### namespace: https://gist.github.com/davidkpiano/c907be5a4768e7a066cc
1. Some examples:
```
import React from 'react';

import * as My from './components/my-components.js';

export default class App extends React.Component {
  render() {
    return (
      <div>
        <My.Foo />
        <My.Bar />
      </div>
    );
  }
}
```

## Compare and Contrast Redux Toolkit with Redux “Ducks”
https://dev.to/code_ashish/modular-ducks-a-design-pattern-for-scalable-redux-architecture-4dna#:~:text=The%20duck's%20pattern%20is%20prone,do%20more%20with%20less%20code.
1. Redux toolkit provide you with an opinionated wrapped around redux and lets us do more with not at much code. 
2. Redux Ducks is prone to a circular dependency. This traditional folder-based approach needs you to separate actions, reducers, selectors and other things into several different files which can be pretty confusing when making changes and un-organized 

## Preview
3. What are you most excited about trying to implement or see how it works?
I kinda want to see what the file setup between Redux toolkit and Redux Ducks would be in comparison and how many more files one has to have over the other. It sounds pretty fun with the naming conventions
