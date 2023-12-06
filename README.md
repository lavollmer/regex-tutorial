# regex-tutorial

Matching a Hex Value 

## Summary

The regular expression described in this tutorial is Matching a Hex Value. The tutorial will discuss how a regex, a shorthand for regular expression, is a pattern that describes a set of strings that tests against an input string.

Hex Value Regex Code Example: /^#?([a-f0-9]{6}|[a-f0-9]{3})$/

The tutorial below will discuss anchors, quantifiers, character classes and more. 

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

The regex components of the regex hex value code includes anchors, quantifiers, OR Operator, character classes, grouping, bracket expression, and greedy matches.

### Anchors

Anchors match a specific part of the input string instead of the characters.

* ^ matches the beginning of the input string
* $ matches the end of an input string

As seen below in the hex value regex example, /^# informs the regex engine that the string will begin with the character #. # will be used to determine a hexadecimal value. The $ anchor tells the regex it is the end of the input string.

Hex Value Example: /^#?([a-f0-9]{6}|[a-f0-9]{3})$/

### Quantifiers

The quantifiers determines numbers of characters or expressions to match.

As seen below in the hex value regex example, the quantifier ? indicates that the character # preceding ? is optional. The quantifier {} informs the regex engine how many instances of the preceding information will be searched.[a-f0-9]{6} indicates that there are 6 instances of the preceding [a-f0-9].The regex will allow for 6 string characters that include a lowercase letter a-f and integer between 0-9. [a-f0-9]{3} indicates that are 3 instances of the preceding [a-f0-9].The regex will allow for 3 string characters that include a lowercase letter a-f and integer between 0-9. 

Hex Value Example: /^#?([a-f0-9]{6}|[a-f0-9]{3})$/

### OR Operator

The OR Operator | is a boolean that matches the before or after code snippet(s). In the hex value regex example below, it is saying that a 6 character string (characters made of lowercase a-f or integers 0-9) or 3 character string (characters made of lowercase a-f or integers 0-9) will be allowed. Anything outside those specified character counts will not match.

Hex Value Example: /^#?([a-f0-9]{6}|[a-f0-9]{3})$/

### Character Classes

A regex includes simple characters and special characters. Simple characters are characters that mean exactly what they are. An example would be the alphabet such as "a" means "a". [abcd] is the same [a-d] which specifies a range of characters.

Character classes are specific subsets of characters. Regex will try to match a single character of an input string to a character from a set.

* [] means to match any of the included characters
* . means to match every character
* All characters and special characters located in the [] means they are to be taken for their literal value

In the hex value matching example, this would apply to the [a-f0-9] code snippets. This would mean the single character would have to include the lowercase letters in the span of a-f or the integers span of 0-9.

### Flags

Regexs have optional flags that allow for searching for global searching and case-sensitive searching. Flags are not included in the hex value example.

### Grouping and Capturing

Grouping groups is an expression like this (). In the hex value matching, the grouping treats the multiple characters as a single group. 

### Bracket Expressions

Bracket expressions such as [abc] matches any character in the set. [a-z] means a range of characters that matches any character in the set. In our hex value matching regex, the bracket expression will match a specific expression. The regex will match anything with [a-f0-9] characters.

### Greedy and Lazy Match

Greedy means to match the longest string possible while lazy match means to match the shortest string possible. The quantifier {} is greedy in the hex value matching example which means it will match as many occurrences as possible. 

### Boundaries

We do not have any boundaries in our hex value matching example. 

For general information about boundaries see below:
Word boundry (\b) matches the word character or position at the end of the word. 

A Not Word Boundry (\B) matches the word character or position that is not at the end of the word.

Example:
* d\b would look for the "d" in the word "and"
* d\B would look for the "d" in the word "wide"


## Author

Laura Vollmer is an aspiring fullstack web developer with experience in healthcare and the floral industry. She is working on learning Javascript, Node.js, HTML, CSS, and much more.

Github profile: https://github.com/lavollmer

## Credits

Information was inspired by:

* https://sdsawtelle.github.io/blog/output/regular-expressions-in-python.html
* https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_expressions
* https://regexlearn.com/cheatsheet