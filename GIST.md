# My REGEX Tutorial!

Regular expressions are special patterns used to search for and manipulate text. They can be helpful for tasks like finding specific words or validating input. In this case, the regular expression you provided focuses on checking if an email address is valid by matching specific characters in the address.

## Summary

We will be analyzing the following Regex code: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components

### Anchors

The anchors used are: ^ to start, and $ to finish.

### Quantifiers

In this example, we utilized the "+" symbol as a greedy quantifier to indicate that there should be another sequence to match. Additionally, we employed the "{2,6}" greedy quantifier to specify that the input should consist of a minimum of 2 characters and a maximum of 6 characters.

### Character Classes

In this regular expression, the character class \d is utilized, which specifically matches any digit from 0 to 9 in JavaScript.

### Grouping and Capturing

This example involves capturing information in three distinct groups. Group #1 captures the username of the email account using the pattern [a-z0-9_.-]. The second group captures the domain name or email service, represented by [\da-z.-]. Lastly, the third group captures the domain extension (e.g., .com or .net) using the pattern [a-z.]{2,6}.

### Bracket Expressions

In this example, there are three bracket expressions used to define character sets. Each bracket expression is enclosed within square brackets [] and determines which characters are allowed to be matched.

Bracket Expression #1: [a-z0-9_.-] - This expression includes lowercase letters from a to z, numbers from 0 to 9, underscore (_), period (.), and hyphen (-).

Bracket Expression #2: [\da-z.-] - This expression includes digits (0-9), lowercase letters from a to z, period (.), and hyphen (-).

Bracket Expression #3: [a-z.] - This expression includes lowercase letters from a to z and period (.).

### Greedy and Lazy Match

In this example, we used "+", and "{}" to match as much as possible. If we added a "?" after them, like "+?" or "{}?", it would make the match as short as possible.


## Author

Hey I'm Chris, my portfolio can be found at: chriskillelea.github.io
