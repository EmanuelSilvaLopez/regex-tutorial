# Regex Tutorial!

The regex expression `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/` is used for matching emails. This is a tutorial to explain it and how it can be beneficial to validating emails on different apps.

## Summary
`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/` is used to validate emails to ensure that the field being entered is an email. A regex or regular expression is a sequence of characters that defines a search pattern commonly used in strings.


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
The anchors for this specific expression are `^` and `$` these are meant to mark the beginning and end of the expression.

### Quantifiers
Quantifiers are the characters used to connect one part of the regex to another. Here the quantifiers are `+` which will connect parts of the regex together and `{2,6}`. These are both greedy quantifiers. `{2,6}` Will specify that a range of 2-6 characters for the character set seen before that `[a-z\.]{2,6}` or `[a-z\.]`.

### Character Classes
`\d` is the character class for this regex and specifies the use of any number between 0-9.

### Grouping and Capturing
There are three groups in this regex. The groups are captured with `()`. The first group which captures the email name is `([a-z0-9_\.-]+)` the second group which will capture the email name like 'gmail' as an example will be `([\da-z\.-]+)` and the last one is `([a-z\.]{2,6})` which will capture the dot domain extension.

### Bracket Expressions
Within the groups captured in the last section are bracket expressions. These show what characters or numbers can be matched within `[]`

The first one is `[a-z0-9_\.-]` which includes characters from a-z and numbers ranging from 0-9 and the special characters underscore, periods and hyphens.

The second one is `[\da-z\.-]` which includes `\d` all digits the same `a-z` which is all characters from a-z and periods and hypens.

The third one is `[a-z\.]` which includes characters from a-z and periods.

### Greedy and Lazy Match
As stated in the quantifiers section there were two greedy quantifiers `{}` and `+` these allow the match to go as long as allowed vs lazy match which will close as soon as able to.
## Author

I am an aspiring full stack web developer.

Emanuel Silva-Lopez: Github Repo https://github.com/EmanuelSilvaLopez 
