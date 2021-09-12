# 5 frame works other than react

## 1 Vue Js by google (2020)

## 2 Angular JS by google(2010)

## 3 Ember JS

## 4 Preact JS

## 5 Svelte JS

## What’s the difference between a framework and a library?

* Frameworks and libraries are both code written by someone else that helps you perform some common tasks in a less verbose way.

* A framework inverts the control of the program. It tells the developer what they need. A library doesn’t. The programmer calls the library where and when they need it.

* The degree of freedom a library or framework gives the developer will dictate how “opinionated” it is.

## Document the following Vocabulary Terms

1 Term: a word or expression that has a precise meaning in some uses or is peculiar to a science, art, profession, or subject

2 Rendering : to show (obedience), as due or expected

3 Templates :  In web design, templates help structure your overall design of a web page. They provide you with areas to place pictures and text, or items like navigation bars and other widgets when you're designing a website. Companies like Squarespace have hundreds of different templates that can be used by anyone to help set up a website easier.

4 State : As defined by FOLDOC, state is how something is; its configuration, attributes, condition or information content.
 A component changes from one state to another over time when triggered by some kind of event.

## Preperation material

### The smallest React example looks like this

```React
ReactDOM.render(
  <h1>Hello, world!</h1>,
  document.getElementById('root')
);

```

### JSX

#### it is a syntax extension to JavaScript. We recommend using it with React to describe what the UI should look like

#### React separates concerns with loosely coupled units called “components” that contain both

#### React doesn’t require using JSX, but most people find it helpful as a visual aid when working with UI inside the JavaScript code

#### Example

```React
const name = 'Josh Perez';
const element = <h1>Hello, {name}</h1>;

ReactDOM.render(
  element,
  document.getElementById('root')
);
```

### rendeeing react

#### React elements are plain objects, and are cheap to create

#### Applications built with just React usually have a single root DOM node

#### React elements are immutable. Once you create an element, you can’t change its children or attributes

* [Source Medium by Darlene Tate](https://medium.com/@BuildMySite1/javascript-templating-what-is-templating-7ff49d97db6b)
* State
  * State is the status of a program or an object and is used for coordinating code. For instance functions activating on state changes.
  * [Source Free Code Camp](https://www.freecodecamp.org/news/state-in-javascript-explained-by-cooking-a-simple-meal-2baf10a787ee/#:~:text=State%20describes%20the%20status%20of,instantly%20react%20to%20that%20change.)
