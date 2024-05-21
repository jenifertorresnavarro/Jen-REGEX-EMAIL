# Matching and Email: Regex Tutorial
What is a regex? Regex is short for regular exression. It is a sequence of characters that defines a specific search pattern. In this tutorial you will learn about matching email expressions using JavaScript. We will look at the different parts of regex patterns designed for validation of email addresses. As well as explinations on how each component plays it's part in ensuring email validation. 

## Summary 
The regex components covered in the tutorial are: Anchors, Grouping constructs, Quantifiers, Bracket Expressions, Character Classes, and Character Escapes.
`` /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ ``

## Table of Contents 
- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [Character Escapes](#character-escapes) 

## Anchors 
The reason anchors can be so vital for our code is because it forces a regular expression to find its match at the start and end of the subject text. In other words, it limits how a regex matches a particular string, since it tells the regex engine where matches begin and where they end. 

**Start Anchor ^: Ensures that the pattern matches at the beginning of a string. <br>
End Anchor $: Ensures that the patters matches at the end of the string.**

## Quantifiers 
Quantifiers are meant to quantify how many times a part of a regular expression should be repeated. Whenever you want something to be repeated in a regex, a quantifier is written after it to specify the amount of times it should be repeated. <br>
As an example, + matches one or more ocurrences. when given `` /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/``

## Bracket Expressions 
A more simple term to understand is Bracket Expressions. In Regex they indicate a character range. This character range will match any character in the range. <br>
**Example** <br>
``[a-z0-9_.-]`` <br>
The character will be matched by any lowercase letters a-z and any number 0-9. 

## Character Classes 
Character classes are shorter than regular expressions, they represent specific sets of characters. Meaning you can simplify and shorten regex patterns, this allows patterns to be easier to understand. Simple classes are the most basic form of character classes. It is to simply place a set of characters within square brackets. <br>
**Example** <br>
``[bcr]at``<br>
will match the words "bat", "cat", or "rat" because within the brackets it accepts "b", "c", or "r" as the first character. However the match only succeeds when the first letter matches one of the characters defined by the character class. This also works with range of values. To specify a range, we can insert "-" metacharacter between the first and last character to be matched. <br>
**Example**<br>
``[a-zA-Z]``<br>
Will match any letter of the alphabet: a to z or A to Z. 

## Character Escapes 
Character escapes bring back the original meaning to a character. Since different characters can mean different things especially in code, the backslash is used to give literals back to these characters. It is important when you need to represent characters that cannot be directly typed. <br>
**Example**<br>
``/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/``<br>
Here a backslad is added to the dot in order to match a period within the email address. Without it the dot could be matched with any character. 

## Author
Written by Jenifer Torres. <br>

[Click me to take you to Jenifer's Github](https://github.com/jenifertorresnavarro).


