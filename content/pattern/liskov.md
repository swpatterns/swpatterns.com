---
title: "Liskov"
date: 2021-03-25T10:42:33+01:00
draft: false
pattern_types: ["principle",]
wikipedia: "https://en.wikipedia.org/wiki/Liskov_substitution_principle"
diagramtype: "class"

code: false
---

The Liskov Substitution Principle has the following wording:

> Let $ \phi (x) $ be a property provable about objects $ x $ of type $ T $. Then $ \phi (y) $  should be true for objects $ y $ of type $ S $ where $ S $ is a subtype of $ T $.

The principle stems from a base concept that is "An Interface is a contract". the parts that use this interface either as implementations or instantiators are aware of this and have to respect this concept. 

If a method exposed by a class requires a specific type to be passed as an argument, subtypes must require at at most the same type of parameters or subtypes of it. 

This is almost always true, yet situations can come up where it is required from the user to ignore the priniple because of side effects that can happen within the code if the principle is perfectly applied.