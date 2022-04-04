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

### Anchors
    Anchors are tokens use to match and compare strings within JavaScript. There are two main anchor tokens "^" and "$". The "^" token is used at the beginning of a string while the "$" token is used at the end. Anchors are then used to assert a string into a certain position. Anchors are commonly used to match and compare, to look for patterns. 
    
    let isValid = /^\d\d:\d\d$/.test('12:05');
    console.log(isValid);
    OUTPUT: True

### Quantifiers

    Quantifiers are used to specify the amount of specific characters in a certain string. They are most commonly used to check the amount of numbers, letters in a string. However they can also be used to generate a string, using the quantifiers you specify the amount of numbers, letters, and characters you want in that string.

    string pattern = @"\b91*9*\b";
    string input = "99 95 919 929 9119 9219 999 9919 91119";
    foreach (Match match in Regex.Matches(input, pattern))
   Console.WriteLine("'{0}' found at position {1}.", match.Value, match.Index);

    OUTPUT: 
    // The example displays the following output:
    //       '99' found at position 0.
    //       '919' found at position 6.
    //       '9119' found at position 14.
    //       '999' found at position 24.
    //       '91119' found at position 33.

### OR Operator

    The OR operator looks like "||" and is used to code "or functions" You would use this operator to compare or match strings that are to the left or right of each other. 

    const a = 3;
    const b = -2;

    console.log(a > 0 || b > 0);
    // expected output: true


### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
