# Matching An Email (Regex Tutorial)

Regex is short for regular expressions which is a sequence of symbols expressing a string or pattern. We will briefly look into what they are and how they work and how they can be broken down to understand what is being communicated.

## Summary

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

Above is an example of a Regex. This string of symbols is used for matching an Email. We will go into what is going on in the regular expression to understand what is going on!

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

Anchors do not match any certain character but they do match a position before or after the characters.

In our Regex we are looking at we can see two different anchor which are ^ and $.

^ is the caret anchor. The caret anchor is meant to show the beginning of what is being matched.
$ is the dollar anchor. The dollar anchor does the opposite of the caret and is meant to show the end of the text that is being matched.


### Quantifiers

Quantifies specify how many instances of a character, group, or character class much be present in the input for a match to be found.

In the Regex we are looking at we can see two different quantifiers.T he + quantifier which defines as matching one or more times This will connect the email name and the email service. The other is {2,6} which indicates a match range between 2 - 6 characters.


### Character Classes

A character class will match characters listed within [].

For reference: [\da-z\.-]
\d is the character class that we can see in our example. It will match a single character that is a digit 0 - 9. It only matches single digits. For example "1" would be matched whereas "11" would not.


### Grouping and Capturing

For reference: regex@gmail.com

There are three capturing groups in our regex for email matching: ([a-z0-9_\.-]+), ([\da-z\.-]+) and ([a-z\.]{2,6}). The first capturing group matches the users email name such as regex in the example email. The second capturing group matches to the email service which in this case is gmail. The third capturing group matches to .com.

### Bracket Expressions

We have three bracket expressions in our example:

[a-z0-9_\.-] is matching any letter a - z. It also matches characters 0 - 9 along with "_", "-" and ".".
[\da-z\.-] is matching a single digit 0 - 9, any character in the range of a - z, "." and ".".
[a-z\.] is matching any character a - z and ".".

### Greedy and Lazy Match

Greedy means to match the longest possible string.
Our example includes greedy matching which are + and {}.

## Author

My name is Jordan Edginton and I am working my way to become a full stack developer.
You can view my work at:
https://github.com/JSplish
