---
layout: post
title:      "React Components: What Are They?"
date:       2019-03-08 05:09:50 +0000
permalink:  react_components_what_are_they
---


### What are components?

Understanding components is an essential part of building and understanding React applications. So, what are they? 

Components are essentially JavaScript functions. What sets components apart from JavaScript functions is that they accept props and return React elements. Components allow a developer to break their application into independent, reusable pieces. There are two main types of components, **class** and **functional**, which we'll dive into deeper below.

#### Class components 

Class components, otherwise known as *stateful components*, are components that are written with ES6 class syntax. What sets class components apart from others is its ability to contain logic and its ability to hold state—class components can be thought of as robust and more code-bearing than others.

```
class Hello extends React.Component {
  render(){
    return(
     <>
       <h1>Hello, I’m a class component!</h1>
     </>
    ) }
  }
```

#### Functional components

Functional components are components that are written as functions. These components are otherwise known as *stateless components* because of their lack of state. For functional components, props are optional. What sets them apart from class components is typically their lightweight code and their tendency to be nothing but presentational.

`const Hello = () => <h1>Hello, I’m a functional component!</h1>`

