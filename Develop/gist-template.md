# Title (replace with your title)

Introductory paragraph (replace this with your text)

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

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
Anchors are used to match patterns that appear at the beginning or end of a line or word.

The caret (^) is used to match the beginning of a line. For example, the pattern ^hello will match "hello" only if it appears at the beginning of a line.

The dollar sign ($) is used to match the end of a line. For example, the pattern world$ will match "world" only if it appears at the end of a line.

Example:
const text = "hello world\nhello everyone\nworld hello";
const pattern1 = /^hello/gm;
const pattern2 = /world$/gm;

console.log(text.match(pattern1)); // Output: ["hello", "hello"]
console.log(text.match(pattern2)); // Output: ["world", "hello"]


### Quantifiers
Quantifiers are used to match patterns that occur a specific number of times.

The asterisk (*) is used to match zero or more occurrences of a pattern. For example, the pattern go*d will match "gd", "god", "good", "gooood", and so on.

The plus sign (+) is used to match one or more occurrences of a pattern. For example, the pattern go+d will match "god", "good", "gooood", and so on.

Example:

const text = "gd god good gooood";
const pattern1 = /go*d/g;
const pattern2 = /go+d/g;

console.log(text.match(pattern1)); // Output: ["gd", "god", "good", "gooood"]
console.log(text.match(pattern2)); // Output: ["god", "good", "gooood"]



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


### Flags

### Grouping and Capturing
Grouping constructs are used to group patterns together and apply quantifiers or alternations to them as a group.

Parentheses () are used to group patterns together. For example, the pattern (ab)* will match zero or more occurrences of the string "ab".

The vertical bar (|) is used to match alternative patterns. For example, the pattern (dog|cat) will match either "dog" or "cat".

Example:
const text = "ab abab ababab dog cat";
const pattern1 = /(ab)*/g;
const pattern2 = /(dog|cat)/g;

console.log(text.match(pattern1)); // Output: ["ab", "abab", "ababab", ""]
console.log(text.match(pattern2)); // Output: ["dog", "cat"]



### Bracket Expressions
Expressions using brackets can be utilized to match characters that fall into a particular set or range of characters.

To match a single character from a set of characters, square brackets [] are utilized. As an instance, the expression [abc] will match any of the letters "a", "b", or "c".

By using the caret (^) within square brackets, it is possible to match any character that is not included in the set. For instance, the expression [^abc] will match any character except for the letters "a", "b", or "c".

Example:
```
let text = "apple banana cherry";
let pattern1 = /[aeiou]/g;
let pattern2 = /[^aeiou]/g;

console.log(text.match(pattern1)); // Output: ["a", "e", "a", "a"]
console.log(text.match(pattern2)); // Output: ["p", "p", "l", " ", "b", "n", "n", " ", "c", "h", "r", "r", "y"]
```

## Author

The author is Evgheni Dimov. I found this assignment on regex to be surprisingly interesting, especially given the requirements. Although I initially struggled to find related material, the readme provided me with the necessary tutorial expectations. I was able to navigate through various resources and watch several videos on the internet to find relevant information about the use and impact of regex or 'Regular Expression' in coding. Overall, I feel that this assignment was quite impressive, and I am proud to have been able to complete it.

Evgheni Dimov 
https://github.com/Eugene-Dim