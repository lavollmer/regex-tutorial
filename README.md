# regex-tutorial

Matching a Hex Value 

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

The regular expression described in this tutorial is Matching a Hex Value. The tutorial will discuss how a regex, a shorthand for regular expression, is a pattern that describes a set of strings that tests against an input string.

Code Example: /^#?([a-f0-9]{6}|[a-f0-9]{3})$/

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

### Anchors

Anchors match a specific part of the input string instead of the characters.

* ^ matches the start of the input string
* $ matches the end of an input string

As seen below in the hex value regex example, /^# informs the regex engine that the string will begin with the character #. # will be used to determine a hexadecimal value. 

Anchor Hex Value Example: /^#?([a-f0-9]{6}|[a-f0-9]{3})$/

### Quantifiers

The quantifiers determines numbers of characters or expressions to match.

As seen below in the hex value regex example, the quantifier ? indicates that the character # preceding ? is optional. The quantifier {} informs the regex engine how many instances of the preceding information will be searched.[a-f0-9]{6} indicates that there are 6 instances of the preceding [a-f0-9].The regex will allow for 6 string characters comprised of a letter and integer. [a-f0-9]{3} indicates that are 3 instances of the preceding [a-f0-9].The regex will look for 3 string characters comprised of a letter and integer.

Anchor Hex Value Example: /^#?([a-f0-9]{6}|[a-f0-9]{3})$/

### OR Operator

The OR Operator | is a boolean that matches the before or after code snippet. In the hex value regex example below, it is saying that a 6 character string (characters made of a-z or integers 0-9) or 3 character string (characters made of a-z or integers 0-9) will be allowed. Anything outside those specified character counts will not match.

Anchor Hex Value Example: /^#?([a-f0-9]{6}|[a-f0-9]{3})$/

### Character Classes

A regex includes simple characters and special characters. Simple characters are characters that mean exactly what they are. An example would be the alphabet such as "a" means "a". [abcd] is the same [a-d] which specifies a range of characters.

Character classes are specific subsets of characters. Regex will try to match a single character of an input string to a character from a set.

* [] means to match any of the included characters
* [^]
* . means to match every character
* All characters and special characters located in the [] means they are to be taken for their literal value

### Flags

Regexs have optional flags that allow for searching for global searching and case-sensitive searching. 

### Grouping and Capturing

Grouping groups an expression like this ().

### Bracket Expressions

Bracket expressions such as [abc] matches any character in the set. [a-z] means a range of characters that matches any chracter in the set.

### Greedy and Lazy Match

### Boundaries

Word boundry (\b) matches the word character or position at the end of the word. 

A Not Word Boundry (\B) matches the word character or position that is not at the end of the word.

Example:
* d\b would look for the "d" in the word "and"
* d\B would look for the "d" in the word "wide"

### Back-references

### Look-ahead and Look-behind



## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)

Laura Vollmer is an aspiring fullstack web developer with experience in healthcare and the floral industry.

Github profile: https://github.com/lavollmer

## Credits

Information was inspired by:

* https://sdsawtelle.github.io/blog/output/regular-expressions-in-python.html
* https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_expressions
* https://regexlearn.com/cheatsheet
*