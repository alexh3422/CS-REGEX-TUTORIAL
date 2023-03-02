# REGEX CHEAT SHEET/GUIDE

This cheat sheet/guide is a useful tool that you can reference while coding. 

## Summary

This cheat sheet/guide will cover everything from Anchors to Flags and more! 

Regex (also known as Regular Expressions) can really come in handy when dealing with text such as searching through forms to make sure email addresses are formatted correct. As an example, here is the regex for that -  `/[A-Z0-9._%+-]+@[A-Z0-9-]+.+.[A-Z]{2,4}/igm` 

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

ANCHORS are special characters that are used to match patterns at specific positions in the input string. 

The two most common ANCHORS are the caret " ^ " and the dollar sign " $ ". The caret matches the start of a string, and the dollar sign matches the end of a string. 

EXAMPLE: the regex pattern "^hello" will match any string that starts with "hello", while the pattern "world$" will match any string that ends with "world". 

### Quantifiers

QUANTIFIERS are special characters that can specify how many times a character (or character group) can be matched in a string. 

The asterisk "", the plus sign "+", and the question mark "?" are some of the most common QUANTIFIERS The asterisk will match zero or more occurrences of the preceding character or group, while the plus sign will match one or more occurrences. The question mark will match zero or one occurrence. 

EXAMPLE: "ab" will match any string that has zero or more letter "a"s that are followed by a letter "b"

### OR Operator

OPERATORS are used to build more complex patterns by combining simpler ones. The two most common operators are the alternation operator "|", and the grouping operator "()".

The alternation operator allows you to match either one pattern or another. For example, if you want to match either "dog" or "cat", you can use the regular expression "(dog|cat)".

The grouping operator "()" allows you to group multiple characters or patterns as a single unit, so that you can apply a quantifier or an operator to the entire group. 

EXAMPLE: if you want to match zero or more occurrences of the sequence "abc", you can use the regular expression "(abc)*".

By using these operators, you can create more powerful regular expressions that can match a wider range of patterns.

### Character Classes

CHARACTER CLASSES allow you to search and match any one of a certain set of characters. They are enclosed in square brackets "[ ]", and the characters you place in between those brackets will be your search values.

EXAMPLE: [aeiou] matches any one of the vowels a, e, i ,o, u. 
This can also be done with numbers, [1234] will match any of the numbers 1, 2, 3, 4. 

You can also use a "-" to create a range. 
EXAMPLE: [a-f] will match any one of the letters a through b (note that this is case sensitive, so [A-F] will match any of the capital letters A through F)



### Flags

FLAGS modify the matching process. They're added at the end of a regular expression, and are represented by the letters "i", "g", and "m".

The "i" flag is for case-insensitivity, the "g" flag is for global matching, and "m" flag is for multiline matching. These flags allow you to customize your regex so that you can match a wider range of text.

EXAMPLE: i flag - /dog/i will make the search for the word dog, case-insensitive. 

### Grouping and Capturing

GROUPING and CAPTURING are important features in regex that allow you to group multiple characters or sub-patterns into a single unit using parentheses. 

Capturing groups are used to extract a specific part of a match and save it in a numbered group for later use. These features can help you create more complex regular expressions and extract useful information from text.


### Bracket Expressions



### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
