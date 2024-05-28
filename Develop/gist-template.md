# REGEX TUTORIAL

A regular expression, or regex, is a sequence of characters used to match patterns in text. These expressions are extremely useful for extracting data like phone numbers, emails, etc that follow a specific pattern from text, and they can be used in almost any programming language including JavaScript.

## Summary

In this tutorial I will break down the following regex for matching an email /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ into its basic components. This regex would be useful for validating email input in various applications.

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
Anchors contain symbols like a caret and a dollar sign at the end of the string or \A letter to create bounderies. The \letter suggests the end of the string. Anchors are a way of telling you where you are at in your code. \A refers to the start. The parameters of regex can vary from language to language. Some characters are the same across multiple languages and have the same meaning, but that is not true for all of them.
### Quantifiers
Regex quantifiers include characters like ?,*, +, and items within curly brackets. They are used to determine the number of occurances or number of items, mostly when it comes to incoming data. Hovering over certain parts of a line of code will tell you the purpose of certain quantifiers. For quantifiers, if you look at W3 schools, almost or all of the descriptions for what quantifiers start with “matches any string with” or “matches any string that.” And then in each of the examples they provide, it says more specifics, for example, matches any string with and end at the end of it or that is for the n $ example. Additionally, quantifiers can determine any string that is followed by a specific string. Essentially, quantifiers tell you what to look for to match OR Operator
### OR Operator
Alternation is an example of an OR Operator. It is declared with a the "|" character. For example, in the context of clothing items, if you wanted to find a few things like a shirt, pants, and shoes, you would write shirt|pants|shoes. This requests all 3, getting rid of the need for individual requests.
### Character Classes
Character classes distinguish kinds of characters for example, numbers and digits. You can specify  a range of characters using a dash, For example, a-d would be the same as typing out a,b,c,d.
### Flags
A flag is an optinal parameter to a regex that modifies its behavior of searching. Flags change the default searching behavior of an expression, and is typically denoted using a single lowercase character. There are 6 different flag types, each serving a different purpose.
-(i) ignore casing. makes the expression search case-insensitive.
-(g) global. makes the expression search for all occurances.
-(s) dot all. makes the wild character "." match newlines.
-(m) multiline. makes the bounday characters "^" and "$" match beginning and end of every line instead of the string.
-(y) sticky. makes the expression start searching from the index.
-(u) unicode. makes the expression assume individual characters as code points, not units.
### Grouping and Capturing
Capturing groups subpatterns together, which allows you to apply quantifiers to multiple at once. It memorizes the information about a subpattern so that you can refer to it later.
### Bracket Expressions
Brackets inform the user and program of a set of characters to match, whereas curly braces are used to specify an exact amount of things to match.
### Greedy and Lazy Match
A greedy match (<.+>) will look for the longest possible string, whereas a Lazy match (<>.+?>) will look for the shortest. Using the word "hello" as an example, the greedy method h.+l matches "hell" in 'hello' but the lazy h.+?l matches "hel".
### Boundaries
Using \b, it serves as an anchor that matches at a position called a "word boundary".  \b allows you to perform a “whole words only” search using a regular expression in the form of \bword\b. A “word character” is a character that can be used to form words. All characters that are not “word characters” are “non-word characters”.
### Back-references
Backreferences match the same text as previously matched by a capturing group. Suppose you want to match a pair of opening and closing HTML tags, and the text in between. By putting the opening tag into a backreference, we can reuse the name of the tag for the closing tag. Here’s an example I was able to grab from https://www.regular-expressions.info/backref.html

 <([A-Z][A-Z0-9]*)\b[^>]*>.*?</\1>. 
### Look-ahead and Look-behind
Lookahead and Lookbehind are assertions that coome in positive and negative. 
For example, lookahead-positive (?=) finds expression A where expression B follows, where look-ahead negative (?!) will find expression A where B does not follow.
lookbehind-positive (?<=>) finds expression A where expression B precedes, where look-behind negative (?<!) finds expression A where expression B does not precede.
## Author

Github: [www.github.com/sjastrow92](https://github.com/sjastrow92)

# Sources

- w3 schools on regex components. 
- regex video provided in assignment description.
- stack overflow.


