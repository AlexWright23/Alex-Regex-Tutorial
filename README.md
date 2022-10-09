# regex-tutorial
Regular expressions, regex, is a sequence of characters that define a search pattern.

## Summary
In this tutorial I will explain the basics of email matching regex

Matching an Email example: //^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/


## Regex Components

## Anchors
The two anchors are '^' and '$'. 

'^', Searches any string where the specified pattern occurs at the beginning of the string or line.
'$', Searches any string where the specified pattern occurs at the end of the string or line.

Since our regex has both, each sting must match exactly or it wont match.

## Character Classes
Regex uses charecters classes to match types of charecters.

'.' Searches for ALL, matches any charecter. 
'\d', matches any single digit charecter, it will search for any number (0-9).

## Bracket Expressions
'[]', will match any charecter in the string. 

[a-z\.] matches any charecter a-z.
[\da-z\.-] matches a single digit charecter, 0-9, and any charecter a-z.
[a-z0-9_\.-] matches any charecter a-z, matches any charecter 0-9, and matches charecters'_' and '-'.

## Quantifiers
Used to specify the number of times a charecter is expected to be shown.

'{}', allows a match range between 2-6 charecters for the set of [a-z\.].
'+', allows a match to happen more than once.

## Flags
Flags are the components regex is written inside of.

'm', this indicates multiline code.
'i', this indicates that the search/charecters are case sensitive.
'g', this indicates that it will search for all matches globaly.

## Grouping Constructs
Grouping is done with '()'.

'()', anything set inside the parentheses is a single group.

 ([a-z0-9_\.-]+) 
 ([\da-z\.-]+)
 ([a-z\.]{2,6})

 ## Character Escapes
 Escapes are shown by backslashes, ('\'), used to escape a charecter that might be interpreted differntly.
 
 ([a-z0-9_\.-]+)

 In our code, we have the ('\.'), the single dot represents any charecter, without the '\.' we would be searching for every single charecter possible, which we do not want.

 ## The OR Operator
 '|' is used as an OR operator, can be used to show that you want one result.

 ## Author 
 Alex Wright
 https://github.com/AlexWright23
