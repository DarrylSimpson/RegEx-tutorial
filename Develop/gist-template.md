# RegEx Tutorial

In this I will be giving a tutorial explainging a specific Regex  

## Summary

In this I will be describing this regex /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ , this expression is used for email adresses to make sure that they meet the criteria to be used as an email adress. It assures that theres a certaint format for the text or numbers before the @ sign, and that there can only be a specific text and symbol options after the @ so that you will have no other choice but to type in a valid email adress.

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
- [Author](#author)

## Regex Components
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
### Anchors
Anchors matches a postion of a character in the string itself.
Examples of Anchors are ^,$
^ - the beggining
Ex. "/^([a-z0-9_\.-]" this mathces any string that starts with any letter a-z, 0-9, a "_", ".", or a "-".
$ - the end 
Ex. "\.([a-z\.]{2,6})$/" this matches the end of the expression is a string that contains any letter, and a period, that 
has minimun 2 characters and maximum 6. 

### Quantifiers
Examples of Quantifiers are *, +, ? {number}, {min,max}
* - 0 or more
Ex. "peoples*" matches a string that has people followed by zero or more S, so it matches "people" and "peoples".
+ - 1 or more
Ex. "peoples+" matches a string that has people followed by one or more S, so it matches "peoples" in this scenario.
? - 0 or 1
Ex. "colou?rs?" matches a string that has "colo" with optional "u", "r", and an optional "s", so this would match "color", "colors", "colour", or "colours".
{number} - how long the string is thats being searched.
Ex. "\w{3}" matches any 3 letter word.
{min,max} - minimum string length and the maximum string length searched.
Ex. \w{2,6} matches any word that has a minimum of 2 letters and a maximum of 6 letters.

### OR Operator
OR operators are anything that appears in [], or ().
Ex. [HELLO] will match H or E or L or O. In context with this email expression before the @ there is [a-z0-9_\.-] which means search for any string that has letters a-z or numbers 0-9 or any of the special characters "_\.-". 
Ex 2. (H|E|L|L|O) matches any string that has H or E or L or O.

### Character Classes


### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author
**Darryl Simpson** [GitHub](https://github.com/DarrylSimpson), [Darryl.Simpson0793@gmail.com](mailto:Darryl.Simpson0793@gmail.com)

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
