1.) STUDENT:

Hey CSE15L course staff!
  I am having trouble with my `reverseInPlace()` method method of my ArrayExamples class. It makes sense to me, but I made test cases with appropriate expected outputs, yet the program apparantly doesn't always give the correct output and fails one of these tests. I notice that the test it fails is quite different from the others, such that it requires the method to reverse multiple elements of the arraylist, as opposed to the other tests that only have one element in the arraylist. My guess is that something is perhaps wrong within the boundaries of the for-loop when we switch elements in the reverseInPlace() method.

  Here are pictures for refernce:

  ![Image](ArrayExamples)  

  ![Image](ArrayTests)

  ![Image](Trigger)


------------------------------------------------------------------------------------------------------------------------------------------------------------------------

2.) TA:

  Hey [Student Name].
    Thank you for reaching out! You seem to be on the right track. Take a look at the line where you're swapping the elements. In the loop, you're iterating over the array and assigning each element to the value of the element at the mirrored position (i.e., the position from the end of the array). However, by doing this, you're essentially overwriting the original values before they are assigned to the correct reversed positions. To fix this, you must swap the indices you are assigning/getting assigned to at line 8.
    
    Try doing arr[arr.length - i - 1] = arr[i]

    
------------------------------------------------------------------------------------------------------------------------------------------------------------------------

3.) STUDENT:

   ![Image](BashSuccess)



------------------------------------------------------------------------------------------------------------------------------------------------------------------------

4.)

FILE/DIRECTORY STRUCTURE:
![Image](d2)

----------------------------------------------------------------------------------------------------------------------------------------------------------------

`ArrayExamples.java`
  ![Image](ArrayExamples)

----------------------------------------------------------------------------------------------------------------------------------------------------------------
`ArrayTests.java`
  ![Image](ArrayTests)
  
----------------------------------------------------------------------------------------------------------------------------------------------------------------
`Test.sh`
![Image](TEST2)

----------------------------------------------------------------------------------------------------------------------------------------------------------------

To trigger the bug, we run the following:
![Image](Trigger)


To fix the bug, we change from `arr[i] = arr[arr.length-i-1]` to `arr[arr.length-i-1] = arr[i]`.

----------------------------------------------------------------------------------------------------------------------------------------------------------------
PART 2

I learned how we're able to add a commit message to our GitHub from the terminal space by using the `git add` and  `git commit -m ""`  commands. I think it's cool b/c for my CSE12 PAs, I always see that TAs have a message next to their username on GitHub, and now I know how it's done.


