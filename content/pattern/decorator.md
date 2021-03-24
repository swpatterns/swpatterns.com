---
title: "Decorator"
date: 2021-03-24T10:30:57+01:00
draft: false
pattern_types: ["GOF", "structural"]
wikipedia: ""
diagramtype: "class"
diagram: "[<<abstract>>Component|+operation()],[Component]^[ConcreteComponent|+operation()],[Component]^[<<abstract>>Decorator|wrappedComponent:Component|+operation()],[Decorator]^[ConcreteDecorator|+operation()]"
code: true
---

The Decorator pattern enables us to change the behavior of an object by hiding the contained functions and adding new functionalities around it. It is also a common way to avoid the limits of single inheritance by multiple interface implementations (composition over inheritance). 

## Usage

This pattern finds its typical use in framework development because it enables the layering of functionalities around a core service. 

## Examples

* Caching in HTTP services can be implemented as a decorator pattern by wrapping the http client within a client that analyzes the requested url and prepares a response
* Logging and instrumenting methods can be implmented as a decorator that covers the interactions once for all the possible activities.