# Leetcode 2272. Substring With Largest Variance (Hard)

# Problem

The variance of a string is defined as the largest difference between the number of occurrences of any 2 characters present in the string. Note the two characters may or may not be the same.

Given a string s consisting of lowercase English letters only, return the largest variance possible among all substrings of s.

A substring is a contiguous sequence of characters within a string.

Return the difference between the maximum and minimum scores among marble distributions.

Solution O(N^2)

Create a list of all unique pairs of characters in the string. For each pair iterate throught the string counting the occurences of each. if the first string has more, set both occurrences to 0, if the second string has more compare the difference to the previous most differences. Reverse the string and repeat once, return differences.
