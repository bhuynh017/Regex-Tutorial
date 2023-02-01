# Regex-Tutorial

## Summary

* The term "regex" is an abbreviated term for regular expression. A regular expression (please see example below) is a used various programming languages to search and manipulate text. This usually consist of special characters.

## Example

* As you can see below this is a regex example is a pattern that is used to match URLs.

* <mark>/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/</mark>

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors

*  Anchors in regex focus on special characters that match positions within the string. As you can see with this example: 

/<mark>^</mark>(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?<mark>$</mark>/

* <mark>^</mark>: this caret indicates the start of the line. While this dollar sign <mark>$</mark> indicates the end of the line.

### Quantifiers

* To go further into the breakdown of the regex example. We will focus on quantifiers. Quantifiers are symbols that are used to define the number of occurences that pattern must match. Below the highlighted are the quantifiers in this regex.

* /^(https<mark>?</mark>:\/\/)<mark>?</mark>([\da-z\.-]+)\.([a-z\.]<mark>{2,6}</mark>)([\/\w \.-]<mark>*</mark>)<mark>*</mark>\/?$/

* <mark>?</mark>: this question mark is used to match the https:// and this is matching the occurence of the pattern.

* <mark>*</mark>: this asterisk matches another pattern in this regex expression. This is used to match the path, query string, and fragment identifier of the URL. 

* <mark>{2,6}</mark> Is stating that there are 2 and 6 occurences within the pattern.

### OR Operator

* The OR operator in regular expressions is shown by having a vertical bar "|". It is used to match patterns on either side of the operator. Unfortunately, the regex pattern does not include an OR Operator.

### Character Classes

* Character classes are used to match a set of characters. A good indicator of character classes is that they will begin and end of square brackets. 

* As you can see the highlighted parts of the expression are indicators of a character class.

* /^(https?:\/\/)?(<mark>[\da-z\.-]</mark>+)\.(<mark>[a-z\.]</mark>{2,6})(<mark>[\/\w \.-]</mark>*)*\/?$/

* <mark>[\da-z\.-]</mark> this indicates that there are matches of any digit, lowercase letter, period, or a hyphen.

* <mark>[a-z\.]</mark> this is matching the lowercase and period.

* <mark>[\/\w \.-]</mark> this is matching any word character, space, period, and hyphen.

### Flags

* Flags are used to state additional options that change the way the expression is interpreted and how the match is performed.The regex expression does not include any flags.

### Grouping and Capturing

* Grouping and Capturing is used to group parts of the expression together and gather text match by those groups. Grouping is used by using parentheses. Capturing is useful for extracting specific parts of a match. In our regex expression the following grouping and capturing are highlighted.

* /^<mark>(https?:\/\/)?</mark><mark>([\da-z\.-]+)</mark>\.<mark>([a-z\.]{2,6})</mark><mark>([\/\w \.-]*)*</mark>\/?$/
* <mark>(https?:\/\/)?</mark> This is matching the optional http:// or https:// at the beginning of the URL.
* <mark>([\da-z\.-]+)</mark> This matches the subdomain and captures it as a separate value.
* <mark>([a-z\.]{2,6})</mark> This matches the top-level domain of the URL.
* <mark>([\/\w \.-]*)*</mark> This matches any path or query string.

### Bracket Expressions
* Bracket expressions are also considered character classes and used to match a set of characters in an expression. Bracket expressions are used to match specific characters in a URL.

* /^(https?:\/\/)?(<mark>[\da-z\.-]</mark>+)\.(<mark>[a-z\.]</mark>{2,6})(<mark>[\/\w \.-]</mark>*)*\/?$/ 
* <mark>[\da-z\.-]</mark> This is used to match the subdomain in the URL.
* <mark>[a-z\.]</mark> This is used to match the top-level domain of a URL.
* <mark>[\/\w \.-]</mark> Thi sis used to match any path or query string in the URL.

### Greedy and Lazy Match

* Greedy and Lazy Match are two different modes of matching in an expression. Greedy is the default and it matches as much of the input string as possible. Lazy matches does the opposite and matches as little of the input string as possible. The expression resorts to default and uses greedy match.

### Back-references

* Back-references allow you to match the same text that was matched by a captured group in a previous pattern.

### Look-ahead and Look-behind

* Look-ahead and Look-behind is an expression that permits a user to match a pattern based on what follows

## Author

* This concludes my regex-tutorial. My name is Bryant Huynh I am an aspiring full-stack engineer who currently attends the SMU Bootcamp. My GitHub is https://github.com/bhuynh017 and my email is bhuynh017@gmail.com. I am also including my LinkedIn https://www.linkedin.com/in/bryanthuynh17/. Please feel free to contact me in either platform!