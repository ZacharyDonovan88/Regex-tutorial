# Regex-tutorial

This is a tutorial to help you understand Regex. A Regex (regular expressions) is a string of characters that represent a particular search pattern. When used in code, regex can be used to find specific patterns of characters within a string. It is used regularly to validate input data. 

## Summary

The following code below will be used for the tutorial. We will use particular examples for how the regex components can be used. The code format we are using is for matching and to validate emails correctly.  

Matching Email-

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

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

The anchor is what begins and ends the regex. In the matching email code,

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/,

The anchors are the ^ and the $. These characters are specifically saying that we are searching for code that begins with

^([a-z0-9_\.-]+)

If we are to find a match, the anchor needs to follow certain instructions. It also needs to end with, 

.([a-z\.]{2,6})$.

It needs to begin and finish within the particular parameters inside the code. If the user does not follow the guideline, then the match will be incorrect and won't proceed.


### Quantifiers

Quantifiers is used to calculate how many times required characters needs to be presented in order to have a successful match. For this following regex code example,

([0-9a-z_.\-]+)

this will match any string that contains 0-9, a-z, _, ., or -. The quantifier + means that it has to contain at least one of this in order to have a match.

### Grouping Constructs

### Bracket Expressions

### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
