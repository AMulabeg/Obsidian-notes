---
id: Lecture 2
aliases: []
tags: []
---

- # Development of a #Database's

    - The concept of a #Database is broken down into 3 parts:
        - Means of description:
            - #ER-models
                - Entity relations
                - #Relationship-type
                - #Attribute
            - Integrity Constraint:
                - Local #IC's
                    - Keys
                    - Domains
                - Structural #IC's
                    - #Cardinality's (n:m,1:n.....)
                    - #Totality
            - #EER-models
                - Generalisation
                - Aggregation
        - Methodical
        - 3 Stages of Development
            - Early
                - First #ER-models
            - Middle
                - #IC
            - Late
                - Further Development of #ER-models
                - Protocols of development
            - Basic Concepts of #ER-models
                - #Entity-Types
                - #Relationship-type
                - #Attribute
                - #IC's

- ## Entity Relationship Model

    - #Entity
        - Is an Object of described world
        - It can only be observed via properties and can not be directly represented
    - #Entity-Types are a collection of #Entity's
    - #Relationship is a connection between 2 or more #Entity's
    - #Relationship-type is a group of similar #Relationship's
    - #Attribute's:
        - Represent a characteristic if an #Entity or #Relationship
        - Only contains primitive data structures (e.g. String, Integers)
        - #IC's
            - #Cardinality and #Totality

- ### #Cardinality of #Relationship-type

    - "General: A binary relationship can connect any number of entities of one type with any number of the other type."
    - "“Can”: This means that not every entity has to be connected to another."
    - #Cardinality 1:n
        - An #Entity **can** have multiple #Relationship's
    - #Totality
        - All #Entity-Types **must** have a #Relationship
        - This is represented with a black dot
    - Recursive #Relationship-type's
        - "Entity types can appear more than once in a relationship type"
            - "Accordingly, several edges are drawn"
            - Each edge corresponds to a role
    
