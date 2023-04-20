# Regex Tutorial

A Regex is a nickname for the term regular expression. They define a search pattern allowing you to key in on certain key words, numbers, symbols, etc. I will be going over one now as an example to deconstruct how a regex works.

## Summary

The Regex I'll be going over is the Regex for matching a URL ` /^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/ `. As previously said it will be a good deconstruction of the components that make up a Regex.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)

## Regex Components

### Anchors

An Anchor is something that can match the position of characters before, between, or after in the string. This allows the Regex to detect position instead of character itself. In the URL Regex ` /^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/ `

The anchors are `^` and `$` and so the `^` anchor detects `(https?:\/\/)` and everything after that while the `$` anchor detects `([\/\w \.-]*)*\/?` and everything befor that. Another way to look at it is that the anchors detect the entire string.

### Quantifiers

Quantifiers are used to encompass the minimum and maximum number of characters that your regular expression is searching for. In this case for the URL Regex the quantifiers are `?`, `+`, `{ , }`, and `*`: 
- `https?` - The `?` is the Quantifier here making sure that `https` is matched zero or one time.
- `(https?:\/\/)?` - Same here, the `?` is the Quantifier making sure that `(https?:\/\/)` is matched zero or one time.
- `[\da-z\.-]+` - The `+` is the Quantifier that will make sure that `a-z`, `.`, or `-` is matched at least one or more times.
- `{2,6}` - The `{ , }` is the Quantifier dictating that `[a-z\.]` may only occur for a minimum of two times to a maximum of six times.
- `[\/\w \.-]*` - The `*` is the Quantifier making sure that `[\/\w \.-]` is matched zero or more times.
- `([\/\w \.-]*)*` - You probably guessed right the `*` once again is the Quantifier making sure that `([\/\w \.-]*)` is matched zero or more times.
- `([\/\w \.-]*)*\/?` - We return full circle with `?` being the Quantifier for `([\/\w \.-]*)*\/` or basically the ending in this case making sure the match is happening zero or one time.

### Character Classes



### Grouping and Capturing



### Bracket Expressions



### Greedy and Lazy Match



### Boundaries



### Back-references



## Author

Justin Perry

I'm new to this whole thing, but I've done my research for the Regex, so I think I've done a pretty good job I might say. If you have any questions or corrections you can contact me directly at lilnewday@gmail.com or on Github https://github.com/LilNewday

