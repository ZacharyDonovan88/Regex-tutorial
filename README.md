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


### Bracket Expressions

The expression flags are used following the initial closing forward slash expression.

i ignores case

g is a modifier to perform a global match which finds all matches instead of stopping after the first match. For case-sensitive matches, combine g with the i modifier.

m is a multiline flag enabled to match the start and end of a line, rather than the start and end of a whole string. The anchors used at the beginning and end should reflect what we've learned previously: ^ and $.

s is a global search for whitespace characters within a string

### Character Classes

\d is shown in the matching email code format and what it will match a single letter character, a-z, after the @ sign in the email address. What this will do is ensuring that a letter is matched after the @ in the email and not a number or special character.

### The OR Operator

It is not shown in the format for the given matching email code, but we will still look at the following code.

/^#?([0-9a-f]{6}|[0-9a-f]{3})$/

This is a regular expression for matching a hex code that uses the OR Operator. The code below will match the #.

[a-f0-9]{6} or [a-f0-9]{3} which will match a 6 or 3 character string that contains a compound of 0-9 numbers and a-f letters.


### Flags

To change how an expression is interpreted, expression flags are used following the initial closing forward slash expression.

i ignores case

g is a modifier to perform a global match which finds all matches instead of stopping after the first match. For case-sensitive matches, combine g with the i modifier.

m is a multiline flag enabled to match the start and end of a line, rather than the start and end of a whole string. The anchors used at the beginning and end should reflect what we've learned previously: ^ and $.

s is a global search for whitespace characters within a string

## Author

Zachary Donovan

GitHub URL: https://github.com/ZacharyDonovan88 
