# Regex-Tutorial

Introductory paragraph (replace this with your text)

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors
Anchors are regex tokens that don't match any characters but that say or assert something about the string or the matching process. Anchors inform us that the engine's current position in the string matches a determined location: for example, the beginning of the string/line, or the end of a string/line.

For example in: 

`(?: ?\G|^cats are )((?:silly|cute)(?: |$))`

 the "\G" anchor denotes the beginning of a match, the "^" anchor denotes the start of a string, and the "$" anchor denotes the end of a string`

### Quantifiers
Quantifiers specify how many instances of a character, group, or character class must be present in the input for a match to be found.

For example, if we were to use

`a{3,6}`

to search through the string "a aa aaa aaaa aaaaaaaaaa", it will match with the group of 3 A's, 4 A's, and the first six A's in the last group, since we asked it to match with the character A in instances of 3-6 characters.

### OR Operator
The OR operator, denoted as '|', is used to match one character OR another character.

For example, if we were to use

`^I like (dogs|cats), but not (snakes|spiders).$`

It would match any of the following strings:

- "I like dogs, but not snakes."
- "I like dogs, but not spiders."
- "I like cats, but not snakes."
- "I like cats, but not spiders."

### Character Classes
Character classes allow us to match one out of several characters. It's very useful when looking for matches that may be misspelled or in a different dialect.

For example, if we were to use
`gr[ae]y`

It will match both "gray" as in American English, or "grey" as in British English.

### Flags

A flag is a part of a regex expression that can be seen as a sort of 'filter' option, allowing us to tailor our regex expressions to fit our needs.

For example: 
- The "i" flag changes the search to be case-insensitive, allowing both capital and lowercase characters to return as a match.
- The "g" flag will cause the search to return all matches instead of just the first match.

### Grouping and Capturing
Grouping allows us to group portions of the regular expression together, giving us the ability to add quantifiers to certain groups, restrict alterations to a part of the expression, or even capturing, which is, in essence, extracting certain portions of the matched string to be used.

To group, we use "()" around the parts of the expression we want to group together.

### Bracket Expressions
Brackets indicate a set of characters to match. Any individual character between the brackets will match, and we can also use a hyphen to define a set.

For example, if we were to use

`[abcd]`

against the string "elephant", it will match the "a" in the string.

### Greedy and Lazy Match
Greedy match mode means that a quantified character will be repeated as many times as possible before stopping. Greedy match will be enabled by default.

A lazy match is the opposite of a greedy match, and will repeat the minimal amount of times before stopping. To create the 

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
