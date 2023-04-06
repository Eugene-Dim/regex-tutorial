# Title (replace with your title)

Introductory paragraph (replace this with your text)

## Summary
^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{2,6})$/

In this article, we'll be discussing a regex expression that is commonly used for validating email addresses. Briefly, this expression seeks a string of letters or numbers, followed by an '@' symbol, another set of letters, a dot, and finally, a string of 2-6 characters in length.

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
Regex: [A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Za-z]{1,}

Example:
regex = r"[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Za-z]{1,}"
email = "eugene@gmail.com"
if reMatch(regex, email):
    print("Correct email address")
else:
    print("Incorrect email address")


### Anchors
^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{2,6})$/

We'll be focusing on two anchors in this expression: the ^ and $ anchors. These anchors are typically used to indicate the beginning and end of a string. ^ - this anchor searches for the start of the string that matches the given criteria, $ - similarly, this anchor ensures that the end of the string adheres to the specified criteria.



### Quantifiers
^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{2,6})$/

Quantifiers are elements within the regex expression that define the number of characters or expressions to match. In our example, we see two quantifiers: the + and the {} brackets. The + signifies that there should be at least one instance of the specified character(s) before the @ symbol. Additionally, {2, 6} indicates that the length of this group must be between 2 and 6 characters.


### OR Operator
The OR operator (^) is used to match one pattern or the other, but not both. It can be used to match mutually exclusive options or alternatives.

The caret (^) separates two mutually exclusive patterns. For instance, the pattern cat^dog will match either "cat" or "dog", but not both.
To group mutually exclusive alternatives, parentheses can be used. For instance, the pattern gray^grey is equivalent to (gray^grey).
Example.
```
let text = "I have a cat and a dog.";
let pattern = /cat|dog/g;

console.log(text.match(pattern)); // Output: ["cat", "dog"];
```
## Character Classes
Character classes allow the regex engine to match one of several characters. For instance, if we want the words grey and gray to both be considered matches, we could use the expression gr[ea]y.

### Flags

### Grouping and Capturing
Grouping and capturing involves enclosing a portion of an expression within parentheses or round brackets. In the provided example, grouping is utilized three times. ([a-z0-9_.-]+) inspects a group that may include lowercase letters, numbers, underscores, hyphens, or periods.


### Bracket Expressions
Bracket expressions employ [] to match user input to the specified characters inside the brackets. For instance, [hHiI] would match hi, hI, Hi, or HI. [a-z] This bracket expression matches any lowercase letter.

### Greedy and Lazy Match
In our given example, we use a greedy regex expression. By using the + quantifier, the engine is able to match one or more instances of the token it quantifies.

## Author

The author is Evgheni Dimov. I found this assignment on regex to be surprisingly interesting, especially given the requirements. Although I initially struggled to find related material, the readme provided me with the necessary tutorial expectations. I was able to navigate through various resources and watch several videos on the internet to find relevant information about the use and impact of regex or 'Regular Expression' in coding. Overall, I feel that this assignment was quite impressive, and I am proud to have been able to complete it.

Evgheni Dimov 
https://github.com/Eugene-Dim 