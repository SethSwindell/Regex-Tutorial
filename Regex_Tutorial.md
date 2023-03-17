# Tutorial on Regular Expression: `/^[A-Za-z\s]+$/

Introduction to regular expressions (regex) and a breakdown of a specific regex.

## Summary

This tutorial will explain the regular expression /^[A-Za-z\s]+$/ which matches strings that only contain alphabetic characters and spaces.

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

The ^ and $ characters are anchors that match the start and end of the string, respectively. In this regex, ^ is used to match the beginning of the string, and $ is used to match the end of the string. This ensures that the regex only matches strings that contain nothing but alphabetic characters and spaces. 

In the example regex, the caret is used at the beginning and the dollar sign is used at the end. This means that the email address must start and end with the specified pattern.

### Quantifiers

The + quantifier matches one or more occurrences of the preceding expression. In this regex, it is used after the character class [A-Za-z\s], which means that the regex matches one or more occurrences of alphabetic characters or spaces.

### OR Operator

The OR operator | can be used to match two or more expressions. In this regex, it is not used.

### Character Classes

The character class [A-Za-z\s] matches any alphabetic character or whitespace character. The uppercase A-Z and lowercase a-z specify all the alphabetic characters. The \s character class matches any whitespace character, which includes spaces, tabs, and line breaks.

### Flags

Flags are used to modify the behavior of the regex engine. The most commonly used flag is the global flag (`g`), which allows the regex to match all occurrences of the pattern in the string.

In the example regex, no flags are used.

### Grouping and Capturing

Grouping and capturing allow you to match multiple expressions and save their matches to be used later. In this regex, there are no groups used.

### Bracket Expressions
Bracket expressions allow you to match any character within a set of characters. In this regex, the bracket expression [A-Za-z\s] matches any alphabetic character or whitespace character.
### Greedy and Lazy Match
Greedy and lazy matching specify how many characters the regex should match. In this regex, the + quantifier is greedy, meaning that it will match as many alphabetic characters or spaces as possible.
### Boundaries
Boundaries are used to match positions rather than characters. In this regex, the ^ and $ anchors are used as boundaries to match the beginning and end of the string, respectively.

### Back-references
Back-referencing allows you to match a previously matched group. In this regex, there are no groups used, so back-referencing is not used.

### Look-ahead and Look-behind
Look-ahead and look-behind are used to match an expression only if it is followed or preceded by another expression. In this regex, there are no look-ahead or look-behind expressions used.
### Author
This tutorial was written by Seth Swindell. https://github.com/SethSwindell
