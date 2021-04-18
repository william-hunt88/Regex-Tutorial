# Email Validation Regex Tutorial

In this tutorial I will wall you through a common email validation using regex. I will break the code down into its functional parts and explain what they are accomplishing.

## Summary

The following code snippet looks intimdating but this tutorial will make it easy to understand and use! There are several kinds of regex operators used and this tutorial will explain each of them in detail. <br>
`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping](#grouping)
- [Bracket Expressions](#bracket-expressions)
- [Greedy Match](#greedy-match)
- [Boundaries](#boundaries)

## Regex Components

### Anchors
`^ and $` <br>
These two operators signify the beginning (^) and end ($) of a string to be matched. 

### Quantifiers
`@`<br>
The @ symbol in between the two bracket expression follows and this checks that the allowed strings are seperated by this symbol. 

### Character Classes
`([\da-z\.-]+)` <br>
The `\da` means any single digit digit is allowed.

### Grouping
`([\da-z\.-]+)` & `([\da-z\.-]+)` <br>
The parentheses are used to seperate groups to be matched.

### Bracket Expressions
`([a-z0-9_\.-]+)` & `([\da-z\.-]+)` <br>
These snippets are what are called bracket expressions and they signifies what characters are allowed in the string. In the first example, any letter or number is allowed as well as an underscore, a period, or a hyphen. In the second exammple, the \d signifies any digit or letter as well as a period or hyphen may be allowed. The () surrounding each expression are for grouping, refer to the [Grouping Section](#Grouping) of this tutorial.

### Greedy Match
`([a-z0-9_\.-]+)@([\da-z\.-]+)` <br>
The plus sign following the group is whats knows as a greedy operator. The plus sign means one or more of the preceding characters are allowed.

### Boundaries
`\`

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
