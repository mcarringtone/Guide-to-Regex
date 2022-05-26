# Regex overview

Regular Expressions also known as REGEX is a sequence of characters that defines a search pattern for text. This will allows you you to filter text. It comes from the mathematical concept of regularset. For example phone numbers are written in umerous ways varying from country to country however, for example using REGEX one can filter out all numbers except for those that are phone numbers in a document, file, or anywhere.

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

Using a standard regex email address I will explain the different concepts within regular expressions.
`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

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

A regex is considered a literal, so the pattern must be wrapped in slash characters (/).

### Anchors

In this REGEX email example the anchors are used in the beginning and the end of the expression to make sure letters and/or numbers are being used. It signifies a string that allows you to match whatever follows the anchor tag for example `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/` in addition a dollar sign can always be considered as an anchor tag.

### Quantifiers

Within REGEX, quantifiers can define how many groups or character classes can be within the text.
For example in the above email address the {2,6} sets the limits to more than two and less than six characters at the end of an email address. Another example of a quantifier is the + symbol. In the email example the plus symbol means how many characters will match the pattern.In the example above , at the beginning of the email at least one number or character must be used as seen in the folling code /^([a-z0-9_\.-]+). The same is true after the @ symbol where at least one number or letter has to be used as seen in the folling code ([\da-z\.-]+).

### Bracket Expressions

Within [] brackets, anything included
In the email above [\da-z\.-]+ at least one requirement will be met. In the email,
caringtonED@gmail.com, matches the [a-z] requirement.

### Character Classes

Character clases also known as character sets, allows REGEX to match one out of several characters.The most common character classes are /d, /s, and /w. These are also known as meta characters.In the example \d matches any number after the @ symbol and before the `.` in the example @([\da-z\.-]+) /d matches any number after the @ symbol and before the `.` .

### The OR Operator

The OR operator is available to use to match characters or expression of either the left or the right of the operator.

### Flags

A flag changes the way a regular expression searches. It makes a regex search in a different way.
In Javascript regex, there are a total of 6 flags, each has a different purpose.

### Character Escapes

The backslash(\) in a regex escapes a character that otherwisewould be intepreted literally.

## Author

I am Carrington Edmondson.
A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
