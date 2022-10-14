# Title (Colin-Regex-Tutorial)

In this tutorial, we will be taking a look at Regex which is regular expression. We will peer into the some of the main components of regex and offer some useful examples and syntax.

## Regex Example
I would like to search and match a telephone number 437-370-4040
Regex: 
`\d{3}[-.]\d{3}[-.]\d{4}`

## Summary
Regex is short for regular expression a programing language. Regular expression is a string of text with a designed search pattern, the string of text can be managed, matched or even replace. Regex is also supported in all of the major scripting languages like Javascript, Python, PHP, and Perl.

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
Anchors are regex tokens. These tokens are not matched with any characters, but they can assert information into the string of text. 
# Syntax: 
- ^ matches the position before the first character in the string. The beginning.
- $ matches right after the last character in the string. The end.

# Example
- `^Before`
- `$After`
- Matches the string Before After


### Quantifiers
Quantifiers are regex features, they are greedy lazy Possessive, sometimes fixed. Quantifiers indicate numbers of characters or expressions to match.
# Syntax: 
- `{ min, max } or {n}` A number is placed inside the curly braces for the search.
- [+] the plus sign means at least one or more
- [*] the multiply means zero or more characters
- [?] the question mark means 0 or 1

### OR Operator
The OR operator in regex is a boolean operator, it executes an operation task if one or more values ore match.
# syntax: 
- `(six|6)` regex six|6 will accept strings "six or "6"

### Character Classes
Regex classes are called character classes. 
The syntax: [ character class begins and ends with the brackets]
Unless noted the rules can change inside the brackets.
character classes are literal.
# Syntax:
- `[0-9]` this indicates match any character 0-9
- `[ ^a-b, A-Z ]` this means matches any letter except A-Z , a-z
- `[.]` the dot is a meta character which means any character

# Example
`\d` matches a digit equivalent to 0-9
abc def g5i jk8

### Flags
Regex flags are modifiers. They are used to modify the behavior of the search.
Flags can be global and they can also ignore.
# Syntax: 
- g indicates (global) and it does not return after the first match. 
- i makes the whole expression case-sensitive.
# Example
- `/Abc/i`

### Grouping and Capturing
Regex uses a pattern of enclosing information inside parentheses. This method is called capturing group.
# Syntax: 
- `(\d?+.)`

### Bracket Expressions
Bracket expressions are a unique type of character class in regex. They match one character out of a set of characters.
# Example
`a-f` will only match a single character in the range a through f
[a-fA-F0-9]
a b c 3 g h 4 ttf

### Greedy and Lazy Match
Greedy describes the type of matching witch continues to search fo a match even after it is found.

### Boundaries
Boundaries or word boundaries are meta-character anchors. It is also a zero length match.
# Syntax: 
- `\b` indicates word boundary

### Back-references
Back references in regex will match the same text which was previously matched by a capturing group.

### Look-ahead and Look-behind
Look-ahead and Look-behind are also known as 'look-around' together.
# Syntax:
- -(?=) 
- (?<=)
# Example
`e(?=m)`
This example will match e only if it is followed by m but m will not be a part of the overall match.

## Author
My name is Colin Nebula and I am a recent graduate of the University of Toronto's coding boot camp as a full stack website developer. I have now added full stack web development to my list of acquired skills.  
(https://github.com/ColinNebula)
