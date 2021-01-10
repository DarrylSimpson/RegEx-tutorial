# Email RegEx Expression Tutorial/Walkthrough

In this I will be going over a (Regular Expression) RegEx defining and identifying a valid email address.

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

### Anchors
Anchors matches a postion of a character in the string itself.

Examples of Anchors are ^,$

^ - the beggining

$ - the end
Ex. "/^([a-z0-9_\.-]" this mathces any string that starts with any letter a-z, 0-9, a "_", ".", or a "-".

In this expression it begins with a "^" which represents what characters should be a the beginning of the expression. So with the ([a-z0-9_\.-]+) code at the beginng means that the expression must begin with those characters. At the end of the expression there is a "$". This "$" signifies that the end of the code needs to be the end of the expression and that expression will qualify for identification.
 

### Quantifiers
Examples of Quantifiers are *, +, ? {number}, {min,max}

In the expression used there are two of these quantifieers being used, the "+" and the "{}" quantifier. The "+" means that everything contained in the expression before it can have an unlimited number of uses.

The other quantifier "{}" shows the minimum and maximum number of characters that part of the expression can be, for this case {2,6} means that this should match a string with at least 2 characters but at most 6.

### OR Operator
OR operators are anything that appears in [], or ().

In each of the three sets of strings, an or operator using "[]" is employed. It signifies that each of the characters in the first set can be any of the approved sets (0-9, a-z, A-Z, _, ., -).

### Character Classes
Examples of character classes are \d, \w, \s

* \d - 0-9, matches any single character that is a digit 



### Flags

This Regex expression makes use of the / g flag, signifying that it will continue searching after the first match. This is useful for finding all matching instances in a grouping.


### Bracket Expressions

The majority of the expression is contained within bracket expressions, all of the [a-z], [0-9] sections are bracket expressions indicating that the ranges indicated are valid expressions.

### Greedy and Lazy Match

Adding the "+" after each of the []s in this expressions shows that this piece of code can exist as many times as possible and only moves on once the next piece of the expression is found, in this case the @ or the ".".

This expression also carries the {} near the end which is also a greedy match as it will take as much as possible until it hits it's upper limit.

## Author
Hello my name is **Darryl Simpson** I am a developer! Check out my [GitHub](https://github.com/DarrylSimpson), I am still at the beggining of my coding journey and learning!

