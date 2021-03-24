---
title: "Composite"
date: 2021-03-23T11:29:42+01:00
draft: false
pattern_types: ["GOF", "structural"]
wikipedia: ""
diagramtype: "class"
diagram: "[Container]<>-children*>[Parent], 
[Parent]^[Container], 
[Parent]^[Leaf]"
---

The Composite Pattern enables us to collect objects into trees that can be easily explored. 
The Parent represents the access point to the tree, where it in fact will be a Container, usually. The container will be able to contain other Container objects or Leaf objects.

Often the sublcasses or the leaves can be instantiated thorugh the various factory patterns. 

## Usage

Typical example is the file system. every folder and every single file are files. Folders contain also other files. 

## Examples

* File system
