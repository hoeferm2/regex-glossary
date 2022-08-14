# regex-glossary

Regular expressions are ......

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

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

- ^[\.\-\)\(]*([0-9]{3})[\.\-\)\(]*([0-9]{3})[\.\-\)\(]*([0-9]{4})$

- A REGEX or regular expression is sequence of characters that defines a search pattern. Comes from the mathematical concepts of regular sets. You could use a word for your regualar expression example my search term is term and that finds lowercase t+e+r+m. This is a 'literal' character search. We can also search 'meta' character searches. In the video i watched the author created a regex to search for phone numbers which are a 3 number then a dash the 3 numbers and another dash and 4 more numbers.
- \d = any digit 0-9
- '-' a dash so that could be 
* Matching a phone number that follows the 3-3-4 format: `\d\d\d-\d\d\d-\d\d\d\d`
to enable regular expressions 
. is a meta that means any character
'*' meta means 0 or more.
.* is a wildcard matches everthing
### Anchors
- ^ this matches the positon  before the first character in the string
- $ represents the end of the string
### Quantifiers
- ` /^[\.-)( ]* ` the * is a quantifier that indicates zero or more occurances of the precedings element, in this case effectively removing any false negatives due to spaces periods dashes or parenthesis.

### Grouping Constructs
- sub expressions 

### Bracket Expressions
- [] indicatess a set of characters to match 
- {} indicated the exact amout of characters in this regex we see {3} amd {4}
- () indicated remembered matches

### Character Classes
- character classes define a set of characters any of which can occur in the input string for the match to succeed
- in my example [(0-9)] measn that if the character is between 0-9 there will be a match
- to link in with curly brackets [(0-9){3}] means that any string of three integers will lead to a match
- including the ^ in the square brackets means that anything that does NOT match the referecened characters will be a match ex . [^aeiou] means anything BUT vowels

### The OR Operator
- The OR operator '|' allows the searcher to create a search with mulitple matches. 
### Flags
- Flags are what enxompasses the scope of your search be that on a global scale or simple multiline
### Character Escapes
- to use a character one must use a backslash \ this indicates that charater following it is a special character
- \t is tab
- \n is new line
## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
