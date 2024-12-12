# seminario-1

## Markdown

- item
- item
- item

1. valor
2. valor
3. valor

| title1 | title2 |
| ------ | ------ |
| a      | b      |

[Markdown](https://docs.github.com/pt/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)

## Plantuml

```plantuml {align="center"}
@startuml
title: Animal example
note "From Duck till Zebra" as n1
class Animal{
    +int age
    +String gender
    + boolean isMammal()
    + void mate()
}
class Duck extends Animal{
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

class Duck
note left: can fly\ncan swim\ncan dive\ncan help in debugging

'para a heranca ficar para o lado
Animal <|- Zebra 

'para a heranca ficar para baixo
Animal <|-- Fish 

@enduml
```
[PlantUML Class Diagram](https://plantuml.com/class-diagram)

## Mermaid

```mermaid {align="center"}
---
title: Animal example
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

[Mermaid Class Diagram](https://mermaid.js.org/syntax/classDiagram.html)


## Markdown Preview Enhanced

[Markdown Preview Enhanced](https://shd101wyy.github.io/markdown-preview-enhanced/#/)


@import "src/Classe.java"