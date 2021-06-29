
# Regex Tutorial for Matching an Email.

A Regular Expression or Regex is a sequence of characters that are used to specify search patterns within a string and
is used as a find and replace or input validator operation.
Regex can be used in search engines, text editors and word processors. Regex is also used in mamy programming languages either
built in or in the form of libraries.

## Summary
The regex we will be describing here in this tutorial is for matching an email : /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

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
Regular Expressions

### Anchors
Regex anchors do not match characters but instead match they match the position before 
or after the characters.
The ^ (Caret Anchor) matches the start of the text.
The $ (Dollar Anchor) matches the ending of the text.

### Quantifiers
Quantifiers identify how many examples of the character, group, or  the character class must be available 
in the code for the match to be found.
In this example we are seeing the + symbol which tells us there is another sequence to be matched.
2,6 are being used as a greedy quantifier as intergers, so the Regex tries to match between a min of 2 characters to 4 characters.

### Grouping Constructs
Grouping is a way of handling multiple characters into a single unit, they are made by placing the characters inside a set of ().
The multiple characters captured here in this example are ([a-z0-9_\.-]+) which is the email username.
The next set ([\da-z\.-]+) represents the email domain and the last ([a-z\.]{2,6}) would be the captured .com


### Bracket Expressions
Bracket expressions show a set of characters that will be matched within the []. Any single character within  the brackets will match,
also a hyphen can be used to define the group.
Being shown here is  the first set of brackets [a-z0-9_\.-] this is displaying case sensitive letters from a-z as well as numbers from 0-9 
and a hypen and period.
The second set of brackets [\da-z\.-] is displaying all digits and case sensitive from a-z along with the hypen and period.
The third set of brackets contain [a-z\.] displaying case sensitive characters and a period.

### Character Classes
A character class is the name that matches any given symbol from a certain set.
The character class can also find and remove anything that is not a number.
\d- is being used in the matching Email example as a digit from 0-9.

### The OR Operator


### Flags
A flag is an option that can be added to a plain expression to help it search in a different way.
A flag is shown as a single letter character, and it has a different job in modifying an expression's search behaviour.
I do not one is being used here in this Email example.

### Character Escapes
To use a special character as if it were a regular one attach a \ to it.
Eample \d, \., ect... this is called Escaping the character.

Authored by Paul Turner. I am a videographer/graphic artist who is aspiring to add front end developer to my arsenal.
Github link : https://github.com/Pgturn68/Regex-Tutorial
