# Email Validation Regex Tutorial

A regular expression (regex or regexp) is a sequence of characters that defines a search pattern. These patterns are often used for string-searching algorithms for "find" or "find and replace" operations on strings, or for input validation.

## Summary

The following regular expression can be used to validate a user's email address:
`/^([a-z0-9_.-]+)@([\da-z.-]+)\.([a-z.]{2,6})$/`

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [About the Author](#about-the-author)

## Regex Components

Regular expressions can contain multiple components to accomplish different tasks. This expression contains the following components:

1. Anchors:

`^`: Asserts the position at the start of the string.
`$`: Asserts the position at the end of the string.

2. Quantifiers:

`+`: Matches the preceding element one or more times.
`{2,6}`: Specifies that the preceding element must occur at least 2 times and at most 6 times.

3. Character Classes:

`\d`: Matches any single digit.
`.`: Matches a literal period.

4. Grouping and Capturing:

`()`: Creates a capturing group that can be treated as a single unit.

5. Bracket Expressions:

`[]`: Defines a set of characters to match.

### Anchors

Caret (^)
The caret `^` asserts the position at the start of the string. In this regex, it ensures that the email address begins with the characters defined in the first grouping.

Dollar ($)
The dollar sign `$` asserts the position at the end of the string. In this regex, it ensures that the email address ends with the characters defined in the last grouping.

### Quantifiers

Quantifiers specify the number of occurrences of a character or a group of characters.

Plus (+)
The plus `+` quantifier matches the preceding element one or more times. In this regex, it applies to [a-z0-9_.-] and [a-z0-9.-].

Curly Braces ({})
Curly braces `{n,m}` specify a minimum and maximum number of occurrences. In this regex, `{2,6}` specifies that the preceding element must occur at least 2 times and at most 6 times.

### Character Classes

Character classes match any one of a set of characters.

Digits (\d)
`\d` matches any single digit.

Period (.)
`.` matches a literal period.

### Grouping and Capturing

Parentheses `()` create a capturing group that can be treated as a single unit.

In this regex:

`([a-z0-9_.-]+)` matches the user part of the email address.
`([\da-z.-]+)` matches the domain part of the email address.
`([a-z.]{2,6})` matches the top-level domain.

### Bracket Expressions

Bracket expressions `[]` define a set of characters to match.

`[a-z0-9_.-]`
Matches any lowercase letter, digit, underscore, period, or hyphen.

`[\da-z.-]`
Matches any digit, lowercase letter, period, or hyphen.

## About the Author

This tutorial was created by Ernesto Hidalgo, a Full Stack Web Developer, passionate about helping others learn regex. You can find more about me on my [GitHub](https://github.com/seokhh10) profile.
