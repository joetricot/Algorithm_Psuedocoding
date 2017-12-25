## Practice Pseudocoding

In groups of 4, each person should take a turn attempting to solve the problems below **with pseudocode**. The other group members can act as support, and provide feedback.

**Take a picture of each solution when you are finished. Include all of your group's pictures in a pull request. Only one pull request per group is required.**

1. FizzBuzz

  "Write a program that prints the numbers from 1 to 100. But for multiples of three print “Fizz” instead of the number and for the multiples of five print “Buzz”. For numbers which are multiples of both three and five print “FizzBuzz”

2. A function that reverses a string

3. A function that takes a number as an argument and returns an array with three items: the number + 1, the number + 2, the number + 3

4. A function that takes an array and a function as two arguments, and returns a new array after calling the function on each item in the original array. E.g. if the original array is [0, 1, 2] and the function is plusOne, the new array will be [1, 2, 3]

5. A function that returns the second highest number in an array of integers.

6. Given a non-empty string and an int N, return the string made starting with char 0, and then every Nth char of the string. So if N is 3, use char 0, 3, 6, ... and so on. N is 1 or more.

7. Given an array of ints, return the string "even" if there are more even elements in the array, or "odd" if there are more odd elements in the array.

8. Given two strings, word and a separator sep, return a big string made of count occurrences of the word, separated by the separator string. For example, repeatSeparator("Word", "X", 3) returns "WordXWordXWord".

9. Given 2 int values greater than 0, return whichever value is nearest to 21 without going over. Return 0 if they both go over.

10. Given 3 int values, a b c, return their sum. However, if one of the values is 13 then it does not count towards the sum and values to its right do not count. So for example, if b is 13, then both b and c do not count.

  - luckySum(1, 2, 3) -> 6
  - luckySum(1, 2, 13) -> 3
  - luckySum(1, 13, 3) -> 1

11. Given a string and an int n, return a string made of the first n characters of the string, followed by the first n-1 characters of the string, and so on. You may assume that n is between 0 and the length of the string, inclusive (i.e. n >= 0 and n <= str length).

  - repeatFront("Chocolate", 4) -> "ChocChoChC"
  - repeatFront("Chocolate", 3) -> "ChoChC"
  - repeatFront("Ice Cream", 2) -> "IcI"

12. Given an array length 1 or more of ints, return the difference between the largest and smallest values in the array.

  - bigDiff([10, 3, 5, 6]) -> 7
  - bigDiff([7, 2, 10, 9]) -> 8
  - bigDiff([2, 10, 7, 2]) -> 8

13. We have triangle made of blocks. The topmost row has 1 block, the next row down has 2 blocks, the next row has 3 blocks, and so on. Compute the total number of blocks in such a triangle with the given number of rows.

  - triangle(0) -> 0
  - triangle(1) -> 1
  - triangle(2) -> 3

14. We have an array of heights, representing the altitude along a walking trail. Given start/end indexes into the array, return the sum of the changes for a walk beginning at the start index and ending at the end index. For example, with the heights [5, 3, 6, 7, 2] and start=2, end=4 yields a sum of 1 + 5 = 6. The start and end index will both be valid indexes into the array with start <= end.

  - sumHeights([5, 3, 6, 7, 2], 2, 4) -> 6
  - sumHeights([5, 3, 6, 7, 2], 0, 1) -> 2
  - sumHeights([5, 3, 6, 7, 2], 0, 4) -> 11

15. A magic index in an array of n integers is defined to be an index i such that a[i] === i. Given a sorted array of distinct integers, write a method to find a magic index, if one exists, in a given array.

16. Suppose we could access yesterday's stock prices as an array, where:

  - The indices are the time in minutes past trade opening time, which was 9:30am local time.
  - The values are the price in dollars of Apple stock at that time.

  So if the stock cost $500 at 10:30am, stockPricesYesterday[60] = 500. You are going to write versions of a method that takes stockPricesYesterday and returns the best profit I could have made from 1 purchase and 1 sale of 1 Apple stock yesterday. No "shorting" - you must buy before you sell. You may not buy and sell in the same time step (at least 1 minute must pass).

  For example:

  ```
  stockPricesYesterday = [10, 7, 5, 8, 11, 9];

  getMaxProfit(stockPricesYesterday);
  // returns 6 (buying for $5 and selling for $11)
  ```

17. Write a function that takes a string and reverses the order of words but not the characters within the words. E.g. "The eagle has landed" becomes "landed has eagle The".

18. The "key" array is an array containing the correct answers to an exam, like {"a", "a", "b", "b"}. The "answers" array contains a student's answers, with "?" representing a question left blank. The two arrays are not empty and are the same length. Return the score for this array of answers, giving +4 for each correct answer, -1 for each incorrect answer, and +0 for each blank answer.
  - scoreUp(["a", "a", "b", "b"], ["a", "c", "b", "c"]) → 6
  - scoreUp(["a", "a", "b", "b"], ["a", "a", "b", "c"]) → 11
  - scoreUp(["a", "a", "b", "b"], ["a", "a", "b", "b"]) → 16

19. Find the first non-repeated character in an array of characters

20. Given three ints, a b c, return true if one of them is 10 or more less than one of the others.

21.
Given two arrays of ints sorted in increasing order, outer and inner, return true if all of the numbers in inner appear in outer. The best solution makes only a single "linear" pass of both arrays, taking advantage of the fact that both arrays are already in sorted order.

  - linearIn([1, 2, 4, 6], [2, 4]) → true
  - linearIn([1, 2, 4, 6], [2, 3, 4]) → false
  - linearIn([1, 2, 4, 4, 6], [2, 4]) → true
