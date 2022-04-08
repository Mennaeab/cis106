# Week report 6

# Summary of the presentation
In this week's lecture we covered wildcards, these include 3 types; *,? and [] and what they are and do. As well as the brace expansion

## Wildcards
Wildcards are symbols that are used to replace of represent one or more characters in a file name.

**Types of wildcards**

| symbol | what it does | Example |
|--------|--------------|---------|
|  *     | is used to match zero to any number of characters | ls*.pdf |
| ?      | is used to match only 1 character | ls program?.py |
| [ ]     | is used to match 1 character from a given set | ls document[A-Z].doc|

## Brace expansion and how to use it

The brace expansion allows us to create a whole directory structure in a single command 

**Example**:
> mkdir -p videos/{dogs,cats}/{breeds,adoption,info}

**The directory should then look like this** :

videos/
├── dogs
│   ├── breeds
|   ├── adoption
│   └── info
└── cats
|    ├── breeds
|    ├── adoption
|    └── info

