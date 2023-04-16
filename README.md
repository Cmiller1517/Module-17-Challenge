# 10 Object-Oriented Programming: Team Profile Generator

#### Table of Content

[Character-Group-1] (#character-group-1)


## Deployed Asset



## Criteria Chosen 

 Matching an Email: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

## Character Group 1

([a-z0-9_\.-]+)

This first charcter set for the Email, it looks for any letter characters in the alphabet from a-z first, then letters between 0 and 9. the "_" funcation matches any blank characters, and the "\." function matches a "." character.

The "+" at the end merges the first character group and the second character group. (Quantifier)

## @ Character

This simply looks for a "@" charcter within the email

## Character Group 2

([\da-z\.-]+)

This character group firstly uses "\d" to match and digit characters between 0-9. It then uses "a-z" to match characters in the range from "a" to "z" in the alphabet. the "\." again matches the  "." character. Finally the "-" character looks for a "-" within the email address.

The "+" at the end merges the first character group and the second character group. (Quantifier)

## Character Group 3

([a-z\.]{2,6})

This is the third and final character group the begins with an "a" to "z" character match, followed again by a "\." which matches a "." character. 

The "{2,6}" is another quantifier that matched the preceeding tokens

## $

This macthes the end of the string to finalize the email inputed

