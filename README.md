# Process-String-With-Special-Operations-I
Given a string s containing lowercase English letters and the special characters *, #, and %, process the string from left to right to build a new string called result.
Problem Statement

You are given a string s consisting of lowercase English letters and the special characters *, #, and %.

Build a new string result by processing s from left to right according to the following rules:

Lowercase letter → Append it to result.
* → Remove the last character from result if it exists.
# → Duplicate the current result and append it to itself.
% → Reverse the current result.

Return the final string after processing all characters.

Approach

Use a string result to simulate the operations:

If the current character is a lowercase letter, append it.
If it is *, remove the last character using pop_back().
If it is #, duplicate the string using result += result.
If it is %, reverse the string using reverse().

After processing all characters, return result.
