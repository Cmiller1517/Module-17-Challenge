# 17 Computer Science for JavaScript: Regex Tutorial
A Regex, or regular expression, is a set sequence of characters that are used to filter a search. The characters in a RegEx define specific parameters in which the expression will use to find certain patterns of characters within a string. Each component has a specific function, which I will be explaining for this assignment

## Summary

In my example, I will be explaining the structure for matching an email. 

The following Regex is for matching an email:

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`


## Table of Content

* [Character Group 1](#character_group_1)
* [@ Character](#@_character)
* [Character Group 2](#character_Group_2)
* [Character Group 3](#chacter_group_3)
* [Ending Character](#ending_character)

### Quantifiers

These quantifiers simply specift a number of groups, and are expressed using "*", "+", "?" and "{}"

in our example, the email uses a "+" quantifier, which in order to match, the email must include atleast 1 of the following character outline in the character set.

 
## Grouping Constructs

Grouping breaks down the expression into sub espressions. Parentheses () are used to capture groups. Each group of the RegEx must meet the parameters seperately in order to be a match.



### Character Group 1

([a-z0-9_\.-]+)

This first charcter set for the Email, it looks for any letter characters in the alphabet from a-z first, then letters between 0 and 9. the "_" funcation matches any blank characters, and the "\." function matches a "." character.

The "+" at the end merges the first character group and the second character group. (Quantifier)

### @ Character

This simply looks for a "@" charcter within the email

### Character Group 2

([\da-z\.-]+)

This character group firstly uses "\d" to match and digit characters between 0-9. It then uses "a-z" to match characters in the range from "a" to "z" in the alphabet. the "\." again matches the  "." character. Finally the "-" character looks for a "-" within the email address.

The "+" at the end merges the first character group and the second character group. (Quantifier)

### Character Group 3

([a-z\.]{2,6})

This is the third and final character group the begins with an "a" to "z" character match, followed again by a "\." which matches a "." character. 

The "{2,6}" is another quantifier that matched the preceeding tokens

### Ending Character

The "$" character macthes the end of the string to finalize the email inputed.

