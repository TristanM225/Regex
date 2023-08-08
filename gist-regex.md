# Matching an Email: Regular Expression Exmplanation

Email address are a common form of communication in a digital world. Validating email addresses using regular expressions can help ensure that the input follows a specific format. In this explanation, we'll break down a regular expression used to match email addresses and discuss its different parts.

## Summary

The regex `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/` is used to match validate email addresses. It verifies that an email address consists of a username, followed by the "@" symbol, a domain name, and a top level domain (TLD). I'll explain the various parts of this regex and how to contribute to identifying valid emails.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)
- [Author](#author)

## Regex Components

### Anchors
The `^` and `$` symbols are anchors. They indicate the start and end of the string. In the regex `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/` when you see `^` it means that the pattern you're searching for should begin right at the beginning of the text you're checking. When you see `$` in a regular expression, it means that the pattern you're searching for should be the last thing you find in the text you;re checking.

### Quantifiers
The `+` quantifier specifies that the preceding character or group should appear one or more times. In the regex, both the username and domain name components are followed by the `+` to allow muliple characters.

### Grouping Constructs
Parentheses () are used for grouping sub-patterns together. In the regex, there are three groups used to capture the username, domain name. and TLD separatley.

### Bracket Expressions
Inside the brackets [], character classes define sets of characters that can match at that position. In [a-z0-9_\.-], it matches lowercase letters, degits, underscores, period and hyphen. 

### Character Classes
- [a-z]: Matches lowercase letters.
- [0-9]: Matches digits.
- [\d]: Matches digits (short for [0-9]).
- [\.-]: Matches a period or hyphen.

### The OR Operator
The Verticle bar `|` functions as the OR operator. It's used in charcter classes to match either of the specified characters. In this regex we do not use the OR operator.

### Flags
Flags modify how the regex is proccessed. Common flags include case-insensitive, global matching, etc. However, they are not used in the given regex. You can stack flags after the closing slash.

### Character Escapes
The backslash `/` is used to escape special characters, treating them as literals characters. For instance, `\.` is used to match a literal period.

## Author

Tristan Melillo
- Email: TristanM225@gmail.com
- GitHub: [TristanM225](https://github.com/TristanM225) (Click Me!)
