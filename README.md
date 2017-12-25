# Thinking Algorithmically

## Functions


### LEARNING OBJECTIVES
*After this lesson, you will be able to:*
- Write pseudocode
- Create plan of attack with pseudocode

# Application Logic

## Pseudocode

- Oftentimes in applications you will be solving problems that you have never solved before and are not sure how to do.
- Pseudocode is a technique for tackling these problems without writing real code in an effort to understand the mechanics behind what has to happen programmatically.

## What does that look like?

Pseudocode should describe the entire logic of the algorithm so that programming becomes a task of translating lines of pseudocode into real code.

## Approaching a coding problem

Pseudocode isn't just about writing down the steps that you already know.  It's a tool to help you work through the problem.  Before we can write pseudocode to solve the problem, we need to know the problem.

Here are some steps that can help with problem solving:

- Identify the Problem
- Break it down
- Start small

#### Identify the Problem

- What exactly are we trying to solve?
- What are we delivering?


#### Break it down

- We break the conceptual models down into concrete steps, actionable items.


#### Start small, stay small

Finally, we take some action. This is when we finally start writing code. We fight hard to take small steps, verify that each step achieves what we want, what we expect, before continuing on. If we do too much at once and things break, which they always do, we won't know what is causing the problem. We won't know which part to trust. Humans thrive on easy wins. We need to see forward progress. Remember that.  Use that. Celebrate your wins.


#### Review: the Steps

- Identify the Problem
- Break it down
- Start small


****Q. Where does pseudocode fit in these steps?****

> A. Break it down OR Start small

This process is iterative.  We keep circling around and repeating the earlier steps, just at a different level.

When we first approach a problem, we see the big picture.  "Break it down" gives us big steps.  Then, we take one of those steps and "Break it down".  Now, starting small, we write pseudocode to help illustrate the problem.

Pseudocoding proves that we have *identified* the problem, understand it *conceptually*, and have *broken it down* into *small steps* that we can follow.


#### Syntax for Pseudocode:

There is no one, fixed syntax for pseudocode.  It just needs to be clear, simple, and concise.

If you feel stuck, feel free to use this syntax:

***Referencing: [Introduction to Pseudocode](http://www.slideshare.net/DamianGordon1/pseudocode-10373156)***

* General Structure of Pseudocode

	```text
	PROGRAM <ProgramName>:

	<Do Stuff>

	END.
	```

* Selection: IF/ELSE Statements

	```
	IF <Condition>
		THEN <Statements>;
		ELSE <Statements>;
	ENDIF;

	```
* Iteration: LOOP

	```
	WHILE <Condition>

	ENDWHILE;
	```

---

For each of the following, let's discuss why each pseudocode could be considered "Good" or "Poor" examples of pseudocode:

#### Problem 1 - Determining if a number is even or odd

***Example 1.1:***

```
PROGRAM isEvenOrOdd:
  var num = number;
  IF (num % 2 === 0)
    THEN Print "even";
    ELSE Print "odd";
  ENDIF;
END.
```

***Q. What do we think?***

> A. This is not a great example. Here we are using "var" in our pseudocode when it should read plain english! Also, we should not be using the javascript syntax "===" in our conditional.  Would a non-programmer know that `num % 2 === 0` indicates an even number?

***Example 1.2:***

```
PROGRAM isEvenOrOdd:
  Read number;
  IF number divided by two has no remainder
      THEN Print the number is even;
      ELSE Print the number is odd;
  ENDIF;
END.
```

***Q. What do we think?***

> A. This is better.  It's closer to english.  It clearly states what we are trying to achieve and how, without getting bogged down in the minutia of code.  Even someone that doesn't code can help us check our logic.  Is any number that can be divided by two, cleanly -- without leaving a remainder -- even? Is anything else odd?

#### Problem 2
 A sorted array of consecutive integers is missing a number from the pattern (ie [1,2,4,5] is missing 3). Find the missing number.


```
PROGRAM findMissing
  Read array
  FOR each number in array
    IF current number is not equal to next number - 1
      THEN return current number + 1
    ENDIF
  ENDFOR
END
```


***Q. What do we think?***

> A. We are able to clearly loop through the array and compare the numbers on each iteration.

***


## Extra Advanced Work: Bubble Sort

- [Explanation on how it works](https://www.tutorialspoint.com/data_structures_algorithms/bubble_sort_algorithm.htm)
- How can we design pseudocode to accomplish this algorithm?

### ADDITIONAL RESOURCES

- [Pseudocode](https://en.wikipedia.org/wiki/Pseudocode) (Wikipedia)
- [Introduction to Pseudocode](http://www.slideshare.net/DamianGordon1/pseudocode-10373156)
