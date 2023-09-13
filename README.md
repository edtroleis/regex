# Regex

Regular expression

## Metacharacters

| Metacaracter | Descrição                                    |
| ------------ | -------------------------------------------- |
| .            | any character                                |
| [ ]          | allowed character class                      |
| [^]          | prohibited character class                   |
| ^            | match the beginning of a line                |
| $            | match the end of a line                      |
| /b           | match a word bondary (last word in the line) |

## Quantifiers

| Metacaracter | Descrição                                                    |
| ------------ | ------------------------------------------------------------ |
| ?            | optional                                                     |
| \*           | zero or more                                                 |
| +            | one or more                                                  |
| {m, n}       | matches between m and n                                      |
| {n}          | Matches exactly n occurrences of the preceding character     |
| {n,}         | Matches n or more occurrences of the preceding character     |
| {n,m}        | Matches between n and m occurrences of the preceding element |

## Miscelaneous

| Metacaracter | Descrição                        |
| ------------ | -------------------------------- |
| \            | use special character as literal |
| \|           | or operation                     |
| ( )          | group                            |
| \1...\9      | backrefence from groups          |

## Shorthands

| Shorthand | Valor        |
| --------- | ------------ |
| \d        | [0-9]        |
| \D        | [^0-9]       |
| \w        | [a-zA-Z0-9_] |
| \W        | [a-zA-Z0-9_] |
| \s        | [\t\n\r\f]   |
| \s        | [^\t\n\r\f]  |

# Links

- [Examples](./examples/)
- https://www.tutorialsteacher.com/regex
- https://github.com/cod3rcursos/curso-regex/tree/master
