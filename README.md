# regex-glossary

Regular expressions are expressions that form a search pattern that helps process text

## Summary

- I will be making a regular expression that can find phone numbers in a a multitude of formats
- ^[\.\-\)\(]*([0-9]{3})[\.\-\)\(]*([0-9]{3})[\.\-\)\(]*([0-9]{4})$
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
- A REGEX or regular expression is sequence of characters that defines a search pattern. Comes from the mathematical concepts of regular sets. You could use a word for your regualar expression example my search term is term and that finds lowercase t+e+r+m. This is a 'literal' character search. We can also search 'meta' character searches. I will be creating a search to find numbers and characters.
- \d = any digit 0-9
- '-' a dash so that could be 
. is a meta that means any character
'*' meta means 0 or more.
.* is a wildcard matches everthing
While we could hard code \d\d\d-\d\d\d-\d\d\d\d we will find a more elegant solution to searching phone numbers
### Anchors
- anchors give our searchers a starting point and an ending point
- ^ this matches the positon  before the first character in the string
- $ represents the end of the string
### Quantifiers
- ` /^[\.-)( ]* ` the * is a quantifier that indicates zero or more occurances of the precedings element, in this case effectively removing any false negatives due to spaces periods dashes or parenthesis.
### Grouping Constructs
- sub expressions capture the substrings of an input string.
- 

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
