---
title: "Singleton"
date: 2021-03-15T13:24:44+01:00
draft: false
pattern_types: ["GOF", "Creational"]
wikipedia: "https://en.wikipedia.org/wiki/Singleton_pattern"
diagramtype: "class"

code: true
---

Singleton design pattern enables us to guarantee unicity and a single entry point for services and accesses. Tipically it requires the standard contructor to be hidden in order to avoid direct instantiation, but modern frameworks use this pattern in conjunction with other [creational]({{< ref "/pattern_types/creational" >}}) patterns in order to ease the development of services.
## Usage
Typical usage for the Singleton pattern is the management of a single centralized state with the warranty that nothing that is not part of the singleton interface will touch it.

## Examples
* Angular services are (per default) singletons. These services are instantiated by the framework and can be used directly through Dependency Injection.