# Tutorial on Regular Expression: `/^[A-Za-z\s]+$/

Introduction to regular expressions (regex) and a breakdown of a specific regex.

## Summary

This tutorial will explain the following regex:

^([a-zA-Z0-9._%+-]+)@([a-zA-Z0-9.-]+).([a-zA-Z]{2,})$

sql

This regex is used to validate an email address. 

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

Anchors are used to specify the position of a pattern in the string. The caret (`^`) and the dollar sign (`$`) are the most commonly used anchors. The caret specifies that the pattern must start at the beginning of the string, while the dollar sign specifies that the pattern must end at the end of the string. 

In the example regex, the caret is used at the beginning and the dollar sign is used at the end. This means that the email address must start and end with the specified pattern.

### Quantifiers

Quantifiers are used to specify the number of times a pattern should be matched. The most commonly used quantifiers are `+`, `*`, and `?`. The `+` quantifier matches one or more occurrences of the pattern, the `*` quantifier matches zero or more occurrences of the pattern, and the `?` quantifier matches zero or one occurrence of the pattern.

In the example regex, the `+` quantifier is used to match one or more occurrences of the characters within the square brackets. This means that the characters can appear multiple times in the email address.

### OR Operator

The OR operator (`|`) is used to match one pattern or another. 

In the example regex, the OR operator is not used.

### Character Classes

Character classes are used to match a range of characters. The square brackets (`[]`) are used to specify a character class. 

In the example regex, there are three character classes:

- `[a-zA-Z0-9._%+-]` matches any letter, number, or one of the specified characters (`._%+-`)
- `[a-zA-Z0-9.-]` matches any letter, number, or the period (`.`) or hyphen (`-`)
- `[a-zA-Z]{2,}` matches any two or more letters

### Flags

Flags are used to modify the behavior of the regex engine. The most commonly used flag is the global flag (`g`), which allows the regex to match all occurrences of the pattern in the string.

In the example regex, no flags are used.

### Grouping and Capturing

Grouping and capturing is used to capture parts of the matched pattern. Parentheses (`()`) are used to group and capture the pattern.

In the example regex, there are three groups:

- `([a-zA-Z0-9._%+-]+)` captures the username
- `([a-zA-Z0-9.-]+)` captures the domain name
- `([a-zA-Z]{2,})` captures the top-level domain (TLD

### Bracket Expressions
Bracket expressions, also known as character sets, are used to match any one character from a set of characters. Square brackets ([]) are used to define a bracket expression.

In the example regex, there are three bracket expressions used:

[a-zA-Z0-9._%+-] matches any letter, number, or one of the specified characters (._%+-)
[a-zA-Z0-9.-] matches any letter, number, or the period (.) or hyphen (-)
[a-zA-Z]{2,} matches any two or more letters
### Greedy and Lazy Match
The quantifiers + and * are by default greedy, meaning they match as much as possible while still allowing the overall pattern to match. Adding a ? after a quantifier makes it lazy, meaning it matches as little as possible while still allowing the overall pattern to match.

In the example regex, the + quantifier is greedy and the * quantifier is used with a lazy match (.*?) to match any character zero or more times, but as few times as possible. This is to ensure that the regex matches only valid email addresses.

### Boundaries
Boundaries are used to match the position between a word character (as defined by the regex engine) and a non-word character, or the position between the start/end of the string and a word character.

In the example regex, the ^ anchor matches the beginning of the string and the $ anchor matches the end of the string, making sure that the email address is not a substring of a longer string.

### Back-references
Back-references are used to match a previously captured group. The syntax for back-references is \number, where number is the number of the capturing group.

In the example regex, no back-references are used.

### Look-ahead and Look-behind
Look-ahead and look-behind are used to match a pattern only if it is followed or preceded by another pattern, respectively, without including the pattern in the match.

In the example regex, no look-ahead or look-behind is used.
### Author
This tutorial was written by Seth Swindell.
