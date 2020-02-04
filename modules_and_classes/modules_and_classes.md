# Modules, Classes and Inheritance

By: Briant Gale

Example Repo: [Joke Generator](https://github.com/briantgale/joke_generator)

---------------------------------------------------------------------------

## 1. Introduction

Properly organizing code into modules and classes helps build maintainable code. There's a few high level concepts to understand:

1. When is a module used?
1. When is a class used?
1. When is it important to use class methods? Instance methods?
1. How should we efficiently organize our code?
1. Are there scenarios where it doesn't matter much?

A few things to keep in mind:
* Rails has given us a good model (no pun intended) to follow to keep our code organized, we need to respect that to keep our code clean.
  * A firm understanding of MVC helps up keep our code clean.
  * If it feels like code doesn't fit somewhere, it might be worth finding a better place for it.
  * The rails magic that we use is really just a lesson in efficient code design. E.G. concerns are just modules with a little extra help mixed in.
* Taking extra time out to understand the structure of something means that coming back later will be much simpler.

### Sample Project Requirements

To get started, I wanted to find something fun to build out to demonstrate some clean code. Instead of building a rails app, let's build a gem and take it through a few steps. Here is some acceptance criteria for my joke generator gem:

* A gem that can be used to tell jokes
* Should be able to specify the type of jokes
* Should be able to return the source of the joke
* Should be able to return multiple jokes at once

### Sample Code - First attempt
[Joke Generator, Branch 1](https://github.com/briantgale/joke_generator/tree/1)

* **What are the problems with this code?**
  * Code is duplicated
  * I'm not able to get multiple jokes back in a single call
  * There's no obvious structure
  * Adding a new joke service would be tricky, as there are multiple places to add it. In a larger code based, that wouldn't be as apparent.
* **What are the obvious improvements that can be made?**
  * Organize code into some methods to make it more expandable
  * Build an interface that makes it easier to work with

## 2. Modules

Modules have 2 main purposes:
1. Namespacing code - This helps prevent class names from clashing
1. Mixin functionality - Consolidate common methods into a single place to share with multiple classes



Modules are not instantiated, and therefore cannot have multiple instances.

JokeGenerator:
- All code is built into a single module, so we can't have any kind of instances
- Organizing code is near impossible, and code that is unrelated is all mixed together into a single namespace. As the codebase grows, this will get more confusing to organize, making it tricky to keep our code clean.
- Code is often repeated that could be consolidated.

Easy Improvements:
- Try and consolidate common code shared methods

## Classes




Example:

```ruby
module

```

https://api.chucknorris.io/
https://www.tronalddump.io/
https://icanhazdadjoke.com/api
