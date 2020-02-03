# Modules, Classes and Inheritance
By: Briant Gale

Example Repo: [Joke Generator](https://github.com/briantgale/joke_generator)

## Introduction
This tutorial/training covers the topic of organizing code efficiently by properly using modules and classes.

### Sample Project Requirements

* A gem that can be used to tell jokes
* Should be able to specify the type of jokes
* Should be able to return the source of the joke
* Should be able to return multiple jokes at once

### Sample Code - First attempt
[Joke Generator, Branch 1](https://github.com/briantgale/joke_generator/tree/1)

* **What are the problems with this code?**
* **What are the obvious improvements that can be made?**

## Modules
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
