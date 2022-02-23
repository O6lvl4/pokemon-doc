```mermaid
classDiagram

    class Pokemon {
        Int globalNumber
        String? kindIdentifier
        PokemonSize size
        PokemonType type1
        PokemonType type2
        Boolean shiny
        String nameEN
        String nameJPtoEN
        String nameJP
        PokemonGender? gender
    }
    Pokemon *--> PokemonSize
    Pokemon *--> PokemonType
    Pokemon *--> PokemonGender

    class PokemonSize {
        Int width
        Int height
    }

    class PokemonType {
        String name
    }

    class PokemonGender {
        <<enum>>
        MALE
        FEMALE
    }
```
