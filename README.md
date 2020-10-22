# Open Module Api Documentation

Imagine you have a Swagger documentation (Open Api doc) for every module with source code in your repository. You open a markdown file and see the interface of the module at a glance. No bloating Javadoc/Kdoc anymore. Wouldn't that be great?

Basic mockup:
```
 __________________ ______________________
| Module tree      | Module spec          |
|                  |                      |
|                  |                      |
|__________________|______________________|
```

## Module tree

The module tree is needed in order to navigate through the docs as you used to in your IDE. 

## Module spec

One markdown file should contains the complete public api for a module = Open Api for modules.
First Idea as example SomeClass.md:
```
# Module x

fun root1(a: Int)

...

## Subpackage1 --> should be foldable

fun sub1(): String

fun sub2(): SomeClass --> SomeClass should be a link to its spec.

...

```

## Type spec

All referenced types must be linked and therfore stored as an additional file:
```
# Data Class A

propertyA: String
proertyB: Int
```
