# Email Validation Regex Tutorial

In this tutorial I will wall you through a common email validation using regex. I will break the code down into its functional parts and explain what they are accomplishing.

## Summary
`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

The preceding code looks intimdating but this tutorial will make it easy to understand and use! There are several kinds of regex operators used and this tutorial will explain each of them in detail. <br>

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
These two operators signify the beginning (^) and end ($) of a string to be matched. The character that follows the carat or precedes the dollar sign will be allowed, in this case we have a groups of bracket expressions in the positions, refer to this tutorials [Bracket Expression](#bracket-expressions) section for more info.

### Quantifiers
`([a-z0-9_\.-]+)`<br>
The pkus sign here is whats known as a regex quantifier. This plus sign is saying that one or more of the preceding characters, a [Bracket Expression](#bracket-expressions) in this case, is allowed.

### Character Classes
`([\da-z\.-]+)` <br>
The `\d` means any single digit digit, 0-9, is allowed. The `a-z` means any single lowercase letter is allowed. The plus sign following the [Bracket Expression](#bracket-expressions) means one or more of these allowed characters will match.

### Grouping
`([\da-z\.-]+)` & `([\da-z\.-]+)` <br>
The parentheses are used to seperate groups to be matched. These groups allow you to use regex operators on all of the regex inside the group as done here with the pkus sign 

### Bracket Expressions
`([a-z0-9_\.-]+)` & `([\da-z\.-]+)` <br>
These snippets are what are called bracket expressions and they signify what characters are allowed in the string. In the first example, any letter or number is allowed as well as an underscore, a period, or a hyphen. In the second example, the `\d` signifies any digit or letter as well as a period or hyphen may be allowed. The () surrounding each expression are for grouping, refer to the [Grouping Section](#Grouping) of this tutorial.

### Greedy Match
`([a-z0-9_\.-]+)@([\da-z\.-]+)` <br>
The plus sign following the group is creating whats known as a greedy match. The plus sign means one or more of the preceding characters are allowed, in this case it is allowing one or more of the characters allowed in the preceing [Bracket Expression](#bracket-expressions).

## Author

My name is William Hunt and I am a student in a coding bootcamp learning how to use regex. Please enjoy this tutorial which breaks down a common regex code used for email validation. Check out my Github https://github.com/william-hunt88/. 
