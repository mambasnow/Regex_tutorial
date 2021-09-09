# Regex URL matching

As a web development student I want a tutorial explaining a specific regex, so that I can understand the search pattern the regex defines. 

## Summary

In this tutorial I will explain regular expressions. More specifically how to look up an email using regex.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors
The Anchors are always at the begining and end of the string. 

Use the ^ anchor to match the beginning of the text.
Use the $ anchor to match the end of the text.
Use the m flag to enable the multiline mode that instructs the ^ and $ anchors to match the beginning and end of the text as well as the beginning and end of the line.

example:
let str = 'JavaScript';
console.log(/^J/.test(str));

^ – The caret anchor matches the beginning of the text.
$ – The dollar anchor matches the end of the text.

### Quantifiers
Quantifiers communicate to the regex engine that it MUST match the Quanity of the character or expression to its LEFT. There are two types of Quantifiers; Greedy and Lazy, each type has the same description.

### Grouping Constructs
Grouping constructs delineate the subexpressions of a regular expression and capture the substrings of an input string

(expr)	Match or capture group. Captures the information that matches the expression in parentheses
(?:expr)	Non-capturing group. Groups the contained expressions together (e.g., to apply a quantifier to multiple symbols at once), but does not restrict the information to be captured to only that group.
(?=expr)	Captures information that is followed by the expression if the expression is true and the input matches the pattern that follows this expression.
(?<>)	Named capture group.*
\k<>	Named back reference. *

### Bracket Expressions

A bracket expression is a list of characters enclosed by ‘[’ and ‘]’. It matches any single character in that list.

### Character Classes
Character Classes ensure that a given sequence of characters matches a Larger set of characters.

### The OR Operator
The or operator is a logical operator. Use it in your query to find a or b. 
example:
 (This@email | that@gmail)



### Flags
Flags in (regex) are tokens that modify its behavior of searching

i - ignore - Makes the expression search case-insensitively.

g - Global - Makes expressions search for all occurances

s - Dot All - makes the wild character . match newlines 

m - multiline - Makes the boundary characters ^ and $ match the beginning and ending of every single line instead of the beginning and ending of the whole string.
### Character Escapes

The backslash in a regular expression precedes a literal character. You also escape certain letters that represent common character classes, such as \w for a word character or \s for a space. The following example matches word characters (alphanumeric and underscores) and spaces.

## Author

Joe Nguyen

