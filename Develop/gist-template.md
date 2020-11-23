# Regular Expression || (RegEx) Tutorial

Howdy! Look _below!_

```
/^#?([a-f0-9]{6}|[a-f0-9]{3})$/
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
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## The Regex Components

### Anchors

From the beginning, the first and last symbols are **^** && **$**. These specifically are known as **Line/String Anchors**. They are very special, as they are not meant to match characters, but to match the position of them in a [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) or [\n](https://forum.freecodecamp.org/t/how-to-add-new-line-in-string/17763)

For Example:
```
^abc$
^ - Beginning
$ - End
```
> Matches any string with the combined characters **abc** at the _beginning_ or _end_. 

### Quantifiers



### OR Operator

Also known as an Alternation, OR ```|``` Operators function as a [boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean). Meaning the string can match the expression _before_ or _after_ the operator.

Seen in our Example:
```
[a-f0-9]{6}|[a-f0-9]{3}
```
> Matches any string consisting of lowercase characters between a-f and digits between 0-9 **At 6 total characters {6}** **_OR_** matching any string consisting of lowercase characters between a-f and digits between 0-9 **At 3 total characters {3}**.

### Character Classes


### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

Hi! My name is Cristian. I am a proud Web Developer and have a [GitHub](https://github.com/WoodwindCDT) you can check out! Also, if you wish, contact me at my [Email](mailto:woodwind.turbeville@gmail.com). Thank you :)