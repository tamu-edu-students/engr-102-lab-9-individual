# ENGR 102 Lab Topic 9 (individual)

## Activities
There is one deliverable for this individual assignment. Please submit the following file to Gradescope. Check out the [Frequently Asked Questions](#frequently-asked-questions) below. **Please include the individual header in your ~.py file.**

1. [Small Functions](#small-functions)

## Small Functions
This activity is meant to give you more experience writing functions. Name your file `small_functions.py` and include all of the following parts in **one** file.

For all parts, include the function named **as specified** in your submission. Your program does NOT have to include output, however **you should test your functions on your own device before submitting to Gradescope**. For example, you might include several function calls and print the results. You may make multiple functions within any one of these problems as long as the main function is named accordingly. **Please comment out ALL `input()` statements before submitting.**

<ol type="a">
<li>Write a function named <code>parta</code> that takes in as a parameter one list of numbers and returns the minimum, median, and maximum value of the list, in that order.</li>
<li>Write a function named <code>partb</code> that takes in as parameters two parallel lists: a list of times (in increasing order), and a list of distances traveled by that point in time. The function should return a new list that contains the velocity between consecutive time measurements. The new list should have a length of one less than the original lists.</li>
<li>Write a function named <code>partc</code> that takes in as a parameter one list of numbers and determines if two of the numbers in the list add to 2029. If they do, return the product of the two numbers, otherwise return <code>False</code>.</li>
<li>Write a function named <code>partd</code> that will take in as a parameter a positive integer <code>n</code> and determines if <code>n</code> can be calculated as the sum of 2 or more consecutive positive, even integers. If it can, return a list of the numbers, otherwise return <code>False</code>.</li>
<li>Imagine that you have a spherical bead. In other words, a sphere with a cylindrical hole drilled through the middle: Write a function named <code>parte</code> that will take in as parameters the radius of the sphere and the radius of the hole, and return the volume of the bead. <b>Note:</b> You will probably want to calculate the volume of <a href="https://en.wikipedia.org/wiki/Spherical_cap" target="_blank">a spherical cap</a></li>
<li>Write a function named <code>partf</code> that will take in as parameters a single character, a person's name, company, and email, and returns a single string of the person's digital business card. Use the character as a border, and provide 2 spaces as padding on either side of the longest entry. Your function must <b>return</b> a single string, do NOT print the digital card.

Example using parameters (`"*"`, `"Dr. Ritchey"`,`"Texas A&M University"`, `"snritchey@tamu.edu"`):
```
**************************
*      Dr. Ritchey       *
*  Texas A&M University  *
*   snritchey@tamu.edu   *
**************************
```
</li>
<li>Write a function named <code>partg</code> that takes in as parameters a value of <code>x</code> between -1 and 1 (exclusive) and a value for tolerance. The function should return the series expansion summation for the equation below. Continue to evaluate terms until the absolute value of the term is less than the tolerance.
    
$$\ln \left( \frac{1+x}{1-x} \right) =\sum_{n=1}^{\infty}\frac{2}{2n-1}x^{2n-1}$$

As an example, if `x=0.5` and tolerance is `0.000006`, the first term for `n=1` is

$$\frac{2}{2\ast1-1}0.5^{2\ast1-1}$$

Since this term is greater than the tolerance, add the term to the summation and continue.
</li>
</ol>


## Frequently Asked Questions
1. **Why are there so many problems!?** The only way you're going to get better at writing functions is to write a lot of functions! :)

2. **Do I really have to comment out all of my input() statements?** YES! The autograding code will import your functions, call them one at a time, then check the return value(s). It will NOT provide any inputs. If you get a run time out error, double check that you commented out all of your input statements. Also, you don't even need main code for this assignment. It's just going to call your functions, and ignore your output. BUT, you should definitely test your code on your own device by calling your functions in your main code and checking to make sure they provide the correct return value(s).

3. **Activity 1d can you give me a hint?** You can use more than one parameter in the `range()` function to increment by something other than 1. For example,
```python
for i in range(1, 10, 2):
    print(i, end=' ')
```
will print `1 3 5 7 9 `. This `range()` function starts at `1` (instead of `0`), stops at the number before `10`, and increments by `2`. Or, you could use a while loop and add 2 to each iteration.

4. **Okay, but can you give me another hint?** Solve the problem by hand first! Think about every step you take, even the easy ones! Programming is just telling the computer what to do. Except computers are dumb and need to be told every single obvious step. Remember what we talked about in lecture 5? Develop an algorithm, write out your steps as comments, then add code. If you think before you code, it will take less time!

5. **Activity 1e how do you calculate the bead volume? Why is this so hard???** This question is best answered with a drawing:
![Visual math showing the outline of a bead equals a sphere minus two spherical end caps minus a cylinder. The sphere has radius r, end caps height h and radius a, cylindar height r minus a and radius a.](bead_math.png)
So how do you calculate the volume? Piece it together using the graphical equation! Take the volume of the sphere, and subtract the volume of the end caps and cylinder. The [equations for a spherical cap can be found on Wikipedia](https://en.wikipedia.org/wiki/Spherical_cap).

Have a question you don't see here? Email your instructor!

Based upon Dr. Keyser’s Original<br/>
Revised Fall 2025 SNR
