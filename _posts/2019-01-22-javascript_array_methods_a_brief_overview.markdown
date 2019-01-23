---
layout: post
title:      "JavaScript Array Methods: A Brief Overview"
date:       2019-01-23 02:23:55 +0000
permalink:  javascript_array_methods_a_brief_overview
---


### Destructive vs Non-Destructive

When manipulating and mutating arrays in JavaScript is made easy with the help of array methods. These various methods can be categorized as *destructive* and *nondestructive*, depending on how they ultimately change (or unchanged) the original array that they are used on. *Destructive methods* are said to alter the original array, so that when the array method is chained to it, the original array actually changes into a new, method-made array. *Nondestructive methods* are, unsurprisingly, just the opposite—a *nondestructive method* is said to leave the original array intact, while only changing the returned method-manipulated array.

### Destructive Array Methods

`.pop()`

The `.pop()` method allows you to destructively remove an item from the end of an array, and will return the removed item:

```
const books = [‘You Don’t Know JS’, ‘Cracking the Coding Interview’, ‘Eloquent JavaScript’, ‘Breaking Up The Boys’ Club of Silicon Valley’, ‘The Pragmatic Programmer’];

books.pop();

// => ‘The Pragmatic Programmer’
```


`.shift()`

The `.shift() `method allows you to remove the first element of an array, while mutating the original array. The return value of the `.shift()` method is the element that was removed:

```
const books = [‘You Don’t Know JS’, ‘Cracking the Coding Interview’, ‘Eloquent JavaScript’, ‘Breaking Up The Boys’ Club of Silicon Valley’, ‘The Pragmatic Programmer’];

 books.shift();

// => ‘You Don’t Know JS’
```


`.push()`

The `.push()` method allows you to add elements to the end of an array, returning the length of the new array after doing so. Note that the `.push()` method *will* mutate the original array:

```
const books = [‘You Don’t Know JS’, ‘Cracking the Coding Interview’, ‘Eloquent JavaScript’, ‘Breaking Up The Boys’ Club of Silicon Valley’];

books.push(‘The Pragmatic Programmer’);

// => 5
```


`.unshift()`

The `.unshift() `method allows you to destructively add elements to the beginning of an array. The return value of an `.unshift()`-ed array is the length of the newly mutated array:

```
const books = [‘Cracking the Coding Interview’, ‘Eloquent JavaScript’, ‘Breaking Up The Boys’ Club of Silicon Valley’, ‘The Pragmatic Programmer’];

books.unshift(‘You Don’t Know JS’);

// => 5
```


`.splice()`

While its name is very similar to that of `.slice()`’s, the `.splice()` method *will destructively change or remove elements*  from an array. `.splice()` accepts anywhere from one (the index of the element you’d like to start at) to three (the starting index, the delete count, and the elements you’d like to insert into the arry) arguments. The return value of the `.splice()` method is an array of the elements that were removed from the array:

```
const books = [‘You Don’t Know JS’, ‘Cracking the Coding Interview’, ‘Eloquent JavaScript’, ‘Breaking Up The Boys’ Club of Silicon Valley’, ‘The Pragmatic Programmer’];

books.splice(-1);

// => [‘The Pragmatic Programmer’]
```


### Nondestructive Array Methods

`.slice()`

The `.slice()` method allows you to *nondestructively remove elements* from an array. This method can accept up to two  arguments, one being the starting element’s index, the other being the index before where the `.slice()` will end. If only one argument is given, the `.slice()` method will slice the array from the specified index all the way to the end of the array:

```
const books = [‘You Don’t Know JS’, ‘Cracking the Coding Interview’, ‘Eloquent JavaScript’, ‘Breaking Up The Boys’ Club of Silicon Valley’, ‘The Pragmatic Programmer’];

books.slice(1, 3);

// => [‘Cracking the Coding Interview’, ‘Eloquent JavaScript’]
```

`...` a.k.a. the `Spread Operator `

The `Spread Operator` looks exactly like an ellipsis, and like an ellipsis, the `Spread Operator` *omits* information when crafting a new array, allowing for to less key strokes for developers looking to add elements to an array:

```
const someBooks = [ ‘Breaking Up The Boys’ Club of Silicon Valley’, ‘The Pragmatic Programmer’];

const allBooks = const books = [‘You Don’t Know JS’, ‘Cracking the Coding Interview’, ‘Eloquent JavaScript’, ..someBooks];

someBooks();

// => [ ‘Breaking Up The Boys’ Club of Silicon Valley’, ‘The Pragmatic Programmer’]

allBooks();

// => [‘You Don’t Know JS’, ‘Cracking the Coding Interview’, ‘Eloquent JavaScript’, ‘Breaking Up The Boys’ Club of Silicon Valley’, ‘The Pragmatic Programmer’]
```

