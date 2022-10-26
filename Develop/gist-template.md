# Regex Tutorial

This tutorial will explain what Regex are and how they work. Regex are known as regular expressions which are often used for defining filters. They are a sequence of characters that allow a user to define and determine a specific serach pattern.

## Summary

This tutorial will explain the components of a regex (regular expression) that is used to match a Hex Value. In HTML, a hex value is a color code that has a value which tells the device how much of the color should be displayed. This is an example of a code snippit of regex used to match a hex value: 

/^#?([a-f0-9]{6}|[a-f0-9]{3})$/

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

`/^`#?([a-f0-9]{6}|[a-f0-9]{3})`$/`

Anchors do not match any of the characters in a regex and are used at the start and end of a string expression. In this particular example, referring to the code snippet above, the anchors are `/^` and `$/`.

### Quantifiers

/^#`?`([a-f0-9]`{6}`|[a-f0-9]`{3}`)$/

Quantifiers indicate how many characters are expected and specify how many specific characters must be present in the input in order for there to be a match. The `?` indicates that the expression will match 0 or 1 time. In our specific example, the quantifiers are `{6}` and `{3}` which indicate that the length of the component preceding these quantifiers are `6` and `3`. An example of these are: #FFFFFF and #FFF.

### OR Operator

/^#?([a-f0-9]{6}`|`[a-f0-9]{3})$/

OR operators indicate that the component can match either string that is before or after the `|`. Looking at our example, this shows us that our hex value is either 6 or 3 characters. This is because `[a-f0-9]{6}` indicates `6` and `[a-f0-9]{3}` indicates `3`. 

### Character Classes

/^#?(`[a-f0-9]`{6}|`[a-f0-9]`{3})$/

Character classes tell what type of characters should be expected and are often enclosed within square brackets. The character class for our example is `[a-f0-9]` and this tells us that we should expect to see letters `a-f` and numbers `0-9`. 

### Flags

A flag is an optional component that modifies the default searching behavior of a regex. There are 6 flags that are single lowercase alphabetic characters and each serve a different purpose. They are `i`, `g`, `s`, `m`, `y` and `u`. When looking at our code snippet, it does not appear to have any flags which means that the regular expression will search in the default searching behavior. 

### Grouping and Capturing

Grouping and Capturing (`()`)

### Bracket Expressions

/^#?`([a-f0-9]{6}|[a-f0-9]{3})`$/

Bracket Expressions (`[]`)

### Greedy and Lazy Match

/^#`?`([a-f0-9]{6}|[a-f0-9]{3})$/

### Boundaries

Boundaries (`\b` and `\B`)

### Back-references

Back-references (`\1`)

### Look-ahead and Look-behind

Look-ahead and Look-behind (`(?=)` and `(?<=)`)

## Author

Nicole Verhulp is a recent Psychology and Political Science graduate who is taking a coding bootcamp through UC Davis's continued learning program to complete a certification in full-stack development.

Check out her GitHub repository for all of her previous projects!

[GitHub Profile](https://github.com/nverhulp)
