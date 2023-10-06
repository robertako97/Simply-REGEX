

![Badge for GitHub repo top language](https://img.shields.io/github/languages/top/robertako97/Simply-REGEX?style=flat&logo=appveyor) ![Badge for GitHub last commit](https://img.shields.io/github/last-commit/robertako97/Simply-REGEX?style=flat&logo=appveyor) 

https://github.com/robertako97/Simply-REGEX
# REGEX! You meant Regular Expressions?
### Description
This is a tutorial and introduction to regular expressions, we'll brekdown an email validation `REGEX` to explain more in detail how it works. As for right now you can start by thinking regular expressions as a `query`, truth is that a regular expression is a pattern, a sequence of digits and/or characters that matches the given pattern on a text. 

## Table of Contents
 * [Installation](#installation) 
  * [Usage](#usage) 
 * [Contributing](#contributing) 
 * [Testing](#testing)
 

### Installation
*Steps required to install project and how to get the development environment running:*

No need to install! You can also dive into npm packages to facilitate some tasks.

### Usage
*Instructions and examples for use:*

# Regex Components Guide

A regular expression, often abbreviated as regex, is a powerful tool for pattern matching and manipulation of text.

thing of `REGEX` as a query that matches all that's inside of the expression `/ALL INSIDE HERE!/`:

Some characters are `metacharacters` and have special meanings. Some common metacharacters include `^, $, ., *, +, ?, |, (), [], {}`, etc.
Examples:

- `^`: Anchors the regex at the beginning of the string pattern (or query).
- `$`: Anchors the regex at the end of the string pattern.
- `.`: Matches any single character.
- `*`: Matches zero or more occurrences of the preceding character.
- `+`: Matches one or more occurrences of the preceding character.
- `?`: Matches zero or one occurrence of the preceding character.
- `|`: Acts as an OR operator.

Character Classes:
   Character classes allow you to specify a set of characters within a pair of `[]`.

   Examples:
   - `[abc]`: Matches any one of the characters 'a', 'b', or 'c'.
   - `[0-9]`: Matches any digit from 0 to 9.
   - `[^0-9]`: Matches any character that is not a digit. (See how ^ is a negation now! but it should still be used at the beginning of your string `/^YOUR STRING$/` to concatenate a pattern).

Let's explore the components of a regex using an example, the `regex for matching a hexadecimal color code`:

### `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`


```javascript
1. Anchors "^&"

'^': It marks the start of the string.
    '$': Marks the end of the string.
        
    These anchors specify that the entire string should match the pattern and not just a part of it.

2. Character Classes
        
    [a-f0-9]: Matches any lowercase letter 'a' to 'f' or any digit '0' to '9'.
{6}: Specifies that the preceding character class should occur exactly 6 times (Have 6 digits).
'|': Acts as an OR operator, permitting either the first or the second pattern to match.
{3}: Specifies that the preceding character class should occur exactly 3 times.

3. Quantifiers - Are the ones in control of the number of occurrences of a character or group. As in the example above!:

" {6} and {3} "

Quantifiers define how many times a particular pattern should occur. In this case, it ensures the correct length for both the full and shorthand color codes.

4. Grouping!
        
We can of course use as usual '()': Groups patterns together to help apply quantifiers and alternation to multiple characters as a single unit. In this regex, it groups the two alternatives for full and shorthand color codes.
        
5. Escape Character (This one is tricky...)

The backslash \ is used to escape metacharacters. Aside from marking down the REGEX domains!
        
6. Summary

This hexadecimal color code regex ensures the string starts and ends correctly, containing either a 6-digit or 3-digit hexadecimal color code, that only contains a-z characters and or 1-9 digits! it also handles an optional '#?' character at the beginning.
        
    Understanding these components allows you to read and create regular expressions for various pattern-matching tasks. 
```
### Contributing
*If you would like to contribute, you can follow these guidelines for how to do so:*

Feel free to submit any contribution!

### Features
Regular expressions in `JavaScript` are (you know it) objects, that permits you to pass (yep...) `methods`or more specifically `string methods`.  REGEX can be modifed to match ANY! pattern or combination  including length! This is were `quentifiers` come in handy - letting you {specify, how long will your pattern have to be}, how many specific characters do you need, or even to ignore strings. We can't forget to mention `Object Methods` and `Object Properties`; but you can dive as deep as you need on your script:)

### Testing
*Tests for application and how to run them:* 

N/A

This project is licensed under the Unlicense License.

[![License: Unlicense](https://img.shields.io/badge/license-Unlicense-blue.svg)](https://opensource.org/license/unlicense/)



#### Want to contact me?

GITHUB:

robertako97
 
https://api.github.com/users/robertako97

EMAIL: 

roberto.diazgmx@gmail.com

