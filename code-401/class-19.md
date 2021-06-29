# Automation

- What Does Automation Mean? Automation is the creation and application of technologies to produce and deliver goods and services with minimal human intervention. The implementation of automation technologies, techniques and processes improve the efficiency, reliability, and/or speed of many tasks that were previously performed by humans.
### Regular expression 

- Regular Expressions, often shortened as regex, are a sequence of characters used to check whether a pattern exists in a given text (string) or not.

- re : Python library that supports regular expressions
Basic Patterns: Ordinary Characters: (Links to an external site.)

- Ordinary characters are the simplest regular expressions. They match themselves exactly and do not have a special meaning in their regular expression syntax. Examples are ‘A’, ‘Manar’ , ‘5’. r”Manar”
- Wild Card Characters: Special Characters: (Links to an external site.)

- Special characters are characters that do not match themselves as seen but have a special meaning when used in a regular expression.

> . - A period. Matches any single character except the newline character.

> ^ - A caret. Matches the start of the string.

> $ - Matches the end of string.

> [abc] - Matches a or b or c.

> [a-zA-Z0-9] - Matches any letter from (a to z) or (A to Z) or (0 to 9).

> [^] all the characters that are not in the set will be matched.

> \ - Backslash. :

- If the character following the backslash is a recognized escape character, then the special meaning of the term is taken

- else if the character following the \ is not a recognized escape character, then the \ is treated like any other character and passed through .

> \ can be used in front of all the metacharacters to remove their special meaning

> \w : Lowercase ‘w’. Matches any single letter, digit, or underscore.

> \W : Uppercase ‘W’. Matches any character not part of \w (lowercase w).

> \s - Lowercase ‘s’. Matches a single whitespace character like: space, newline, tab, return.

> \S - Uppercase ‘S’. Matches any character not part of \s (lowercase s).

> \d - Lowercase d. Matches decimal digit 0-9.

> \D - Uppercase d. Matches any character that is not a decimal digit.

> \t - Lowercase t. Matches tab.

> \n - Lowercase n. Matches newline.

> \r - Lowercase r. Matches return.

## function provided by ‘re’
- compile(pattern, flags=0)

- With compile(), you can computer a regular expression pattern into a regular expression object. When you need to use an expression several times in a single program, using compile() to save the resulting regular expression object for reuse is more efficient than saving it as a string. This is because the compiled versions of the most recent patterns passed to compile() and the module-level matching functions are cached.
    - search(pattern, string, flags=0)

- With this function, you scan through the given string/sequence, looking for the first location where the regular expression produces a match. It returns a corresponding match object if found, else returns None if no position in the string matches the pattern. Note that None is different from finding a zero-length match at some point in the string.
    - match(pattern, string, flags=0)

- Returns a corresponding match object if zero or more characters at the beginning of string match the pattern. Else it returns None, if the string does not match the given pattern.
    - findall(pattern, string, flags=0)

- finds all the possible matches in the entire sequence and returns them as a list of strings. Each returned string represents one match.
    - finditer(string, [position, end_position])

- similar to findall() - it finds all the possible matches in the entire sequence but returns regex match objects as an iterator.
    - sub(pattern, repl, string, count=0, flags=0)

- sub() is the substitute function. It returns the string obtained by replacing or substituting the leftmost non-overlapping occurrences of pattern in string by the replacement repl. If the pattern is not found, then the string is returned unchanged.
    - subn(pattern, repl, string, count=0)

- he subn() is similar to sub(). However, it returns a tuple containing the new string value and the number of replacements that were performed in the statement.
    - split(string, [maxsplit = 0])

- This splits the strings wherever the pattern matches and returns a list. If the optional argument maxsplit is nonzero, then the maximum ‘maxsplit’ number of splits are performed.

    - start() - Returns the starting index of the match.
    - end() - Returns the index where the match ends.
    - span() - Return a tuple containing the (start, end) positions of the match.
