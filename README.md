# ENGR 102 Lab Topic 9 (individual)

## Activities
There is one deliverable for this individual assignment. Please submit the following file to Gradescope. Check out the [Frequently Asked Questions](#frequently-asked-questions) below. **Please include the individual header in your ~.py file.**

1. [Small Functions](#small-functions)

## Small Functions
stuff




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
