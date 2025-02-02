# Maximum-Difference-Between-Even-and-Odd-Frequency-I

Problem Statement

You are given a string s consisting of lowercase English letters. Your task is to find the maximum difference between the frequency of two characters in the string such that:

One of the characters has an even frequency in the string.

The other character has an odd frequency in the string.

The maximum difference is calculated as:



If there are no valid odd or even frequency characters, return 0. This ensures that only valid comparisons are made between distinct frequencies.

Solution Approach

1. Count Character Frequencies

Traverse the string and count the occurrences of each character using a dictionary.

This allows efficient frequency tracking for further processing.

2. Separate Odd and Even Frequencies

Iterate over the frequency dictionary and classify counts into:

Odd frequency list (of****): Stores counts that are odd.

Even frequency list (ef****): Stores counts that are even.

3. Compute Maximum Difference

If either of or ef is empty, return 0 (no valid pair exists).

Otherwise, compute the maximum difference as:



This guarantees that we consider the largest possible difference between distinct frequency types.

Problem Statement :


You are given a string s consisting of lowercase English letters. Your task is to find the maximum difference between the frequency of two characters in the string such that:
1. One of the characters has an even frequency in the string.
2. The other character has an odd frequency in the string.
The maximum difference is calculated as:
**Max(Odd Frequency)- Min(Even Frequency)**
If there are no valid odd or even frequency characters, return 0. This ensures that only valid comparisons are made between distinct frequencies.

Solution Approach :


1. Count Character Frequencies:

    1. Traverse the string and count the occurrences of each character using a dictionary.
  
    2. This allows efficient frequency tracking for further processing.

2. Separate Odd and Even Frequencies:

Iterate over the frequency dictionary and classify counts into:

1. Odd frequency list (of****): Stores counts that are odd.

2. Even frequency list (ef****): Stores counts that are even.

3. Compute Maximum Difference:

If either of or ef is empty, return 0 (no valid pair exists).
Otherwise, compute the maximum difference as:

**Max(Odd Frequency)- Min(Even Frequency)**

This guarantees that we consider the largest possible difference between distinct frequency types.

Complexity Analysis :

1. Time Complexity: O(N) , where N is the length of the string.

1. Counting character frequencies takes O(N) .

2. Separating even and odd frequencies takes O(26) =O(1) (since there are at most 26 letters).

2. Space Complexity: O(1) (only stores character counts in a dictionary of at most 26 keys).
3. The algorithm is optimal for large inputs due to its linear time complexity.

Edge Cases Considered :


1. All characters have even frequencies → Output 0.
2. All characters have odd frequencies → Output 0.
3. Mixed frequencies → Compute max difference normally.
4. Single character string → Output 0.
5. Large input strings → Efficient handling within O(N) time.
6. Non-repeating characters → Each character appears once, making the difference minimal.

Summary :


1. Efficient solution using a dictionary for frequency counting.
2. Handles all edge cases properly.
3. Runs in O(N) time, making it optimal for large inputs.
4. Minimal space usage, only storing frequency counts for at most 26 letters.
5. Ensures clear separation of even and odd frequencies, making it easy to compute the required difference.
6. Supports multiple test cases, validating different input scenarios effectively.

This solution provides a clean and efficient way to find the maximum difference between even and odd frequency characters in a given string. 🚀

