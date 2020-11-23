# Regular Expression || (RegEx) Tutorial

Howdy! Look _below!_

```
/^#?([a-f0-9]{6}|[a-f0-9]{3})$/g
```

## Summary

Welcome to my RegEx Tutorial! I have above an example of a [RegEx Expression](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions) meant to match a [Hex Color Value](https://htmlcolorcodes.com/) string. Furthermore, we will dissect and dive into how the expression works in its suited environment.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)

## The Regex Components

### Anchors

From the beginning, the first and last symbols are **^** && **$**. These specifically are known as **Line/String Anchors**. They are very special, as they are not meant to match characters, but to match the position of them in a [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) or [\n](https://forum.freecodecamp.org/t/how-to-add-new-line-in-string/17763).

For Example:
```
^abc$
^ - Beginning
$ - End
```
> Matches any string with the combined characters **abc** at the _beginning_ or _end_.

### Quantifiers

Quantifiers are used to match the scope of a term which precedes it. You **must** place these quantifiers at the end of your desired scope, as they are looking for anything to match before its placement.

```
[a-f0-9]{3}
```
> Matches any string consisting of lowercase characters between a-f and digits between 0-9 **At 3 total characters {3}**.

```
#?
```
> Another Quantifier **?**, matches between 0 and 1 characters of the preceeding expression boundaries **#**.

### OR Operator

Also known as an Alternation, OR ```|``` Operators function as a [boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean). Meaning the string can match the expression _before_ or _after_ the operator.

Seen in our Example:
```
[a-f0-9]{6}|[a-f0-9]{3}
```
> Matches any string consisting of lowercase characters between a-f and digits between 0-9 **At 6 total characters {6}** **_OR_** matching any string consisting of lowercase characters between a-f and digits between 0-9 **At 3 total characters {3}**.

### Character Classes

In the expression, we find character classes are popular! Character classes zone in on any specific character set, combination, any digit, and [more](https://www.regular-expressions.info/charclass.html).

For exmaple:
```
[a-f0-9]
[a-f] - lowercase character set from a through f
[0-9] - digit set from  0-9
```
> Matches any string consisting of lowercase characters between a-f and digits between 0-9. You can combine and manipulate this method to match many different criteria, making it very dynamic!

### Flags

In a RegEx, a Flag can be very influential for how it interprets its search. Flags tend to follow the closing **/** towards the end of an expression.

For Example:
```
$/g
```
> This specific flag searches globally to match _all_ instances rather than stopping after the first match.

### Grouping and Capturing

In the expression, Grouping and Capturing are found using **()** as a means to specify/consolidate which information we want to capture. Any subpattern inside a pair of these parentheses will be captured within a 'group.'

For Example:
```
([a-f0-9]{6}|[a-f0-9]{3})
```
> This specifies _within the brackets_ that we are looking for and extracting strings consisting of a-z and 0-9 criteria and plating them as **Capture Groups**. 

## Author

Hi! My name is Cristian. I am a proud Web Developer and have a [GitHub](https://github.com/WoodwindCDT) you can check out! Also, if you wish, contact me at my [Email](mailto:woodwind.turbeville@gmail.com). Thank you :)