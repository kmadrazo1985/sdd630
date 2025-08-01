# Markdown - Quick Examples

<!-- comment -->

# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6

---
## Formatting
- Example of **Bold Text**
- Example of *Italic Text*
- Example of ~~Strikethrough~~
- Example of <mark>Highlight</mark>
- Example of Subscript H<sub>2</sub>O
- Example of Superscript X<sup>2</sup>
> blockquote
> more blockquotes

---
## Foot Notes
Here's a sentence with a footnote. [^1]

[^1]: This is the footnote.

---
## Term / Definition

term
: definition

---
## Emoji
[Emoji Cheatsheet](https://github.com/ikatyang/emoji-cheat-sheet)

Cheers! :beers:

---
## Ordered List
1. Item 1
2. Item 2
3. Item 3
   1. Indented Item 1
   2. Indented Item 2
   3. Indented Item 3
4. Item 4

---
## Unordered List
- Item 1
- Item 2
- Item 3
    - Indented Item 1
    - Indented Item 2
    - Indented Item 3
- Item 4

---
## Links / Images
[wikiBob](https://gitlab.com/bobby.estey/wikibob/-/blob/master/README.md)

![America's Flagship Seal](https://gitlab.com/bobby.estey/wikibob/-/raw/master/docs/icons/cv64AmericasFlagShip100x100.png)
![America's Flagship Seal](https://gitlab.com/bobby.estey/wikibob/-/raw/master/docs/icons/cv64AmericasFlagShip100x100.png "America's Flag Ship")

---
## Tables
|Column1|Column2|Column3|
|--|--|--|
|Row1Column1|Row1Column2|Row1Column3|
|Row2Column1|Row2Column2|Row2Column3|
|Row3Column1|Row3Column2|Row3Column3|

---
## Task Lists
- [x] Task 1 - completed
- [ ] Task 2 - not completed
- [ ] Task 3 - not completed
- [x] Task 4 - completed

---
## Code Blocks
```
public class CodeBlock {
    public static void main(String[] args) {
        System.out.println("Code Block Example");
    }
}
```



```mermaid
---
title: MermaidJS - Class Diagram - Animal example
---
classDiagram
    note "From Duck till Zebra"
    Animal <|-- Duck
    note for Duck "can fly\ncan swim\ncan dive\ncan help in debugging"
    Animal <|-- Fish
    Animal <|-- Zebra
    Animal : +int age
    Animal : +String gender
    Animal: +isMammal()
    Animal: +mate()
    class Duck{
        +String beakColor
        +swim()
        +quack()
    }
    class Fish{
        -int sizeInFeet
        -canEat()
    }
    class Zebra{
        +bool is_wild
        +run()
    }
```

## Additional Tricks

#### Add a Blank line in a list, put 2 spaces at the end of the line, e.g. Bananas and Green have two spaces at the end

1.  Apples
2.  Bananas  

     1.  Red
     2.  Yellow
     3.  Green  
     
3.  Oranges

