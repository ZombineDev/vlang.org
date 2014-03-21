System Hierarchy
================

Hierarchy is useful for taming system complexity. All modern Hardware and software architectures use hierarchy as a means to provide abstraction. This becomes necessary in order to compensate for [limited capacity of human brain](http://en.wikipedia.org/wiki/The_Magical_Number_Seven,_Plus_or_Minus_Two).

In Vlang hierarchy is all prevaiding. All user-level *Structural Constructs* are hierarchical. Each construct whether statically or dynamically instantiated knows its parent.

![Hierarchy in Vlang](img/hierarchy.png "Hierarchy in Vlang")

Static Hierarchy (and Elaboration)
================

