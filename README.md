1.) STUDENT:

Hey CSE15L course staff!
  I am having trouble with my `reverseInPlace()` method method of my ArrayExamples class. It makes sense to me, but I made test cases with appropriate expected outputs, yet the program apparantly doesn't always give the correct output and fails one of these tests. I notice that the test it fails is quite different from the others, such that it requires the method to reverse multiple elements of the arraylist, as opposed to the other tests that only have one element in the arraylist. My guess is that something is perhaps wrong within the boundaries of the for-loop when we switch elements in the reverseInPlace() method.

2.) TA:

  Hey [Student Name].
    Thank you for reaching out! You seem to be on the right track. Take a look at the line where you're swapping the elements. Notice that

    Try doing arr[i] = arr[arr.length - i - 1]

    


3) Student's Success







4.)

FILE/DIRECTORY STRUCTURE:
![Image](Struc)

----------------------------------------------------------------------------------------------------------------------------------------------------------------

`ArrayExamples.java`
  ![Image](ArrayExamples)

----------------------------------------------------------------------------------------------------------------------------------------------------------------
`ArrayTests.java`
  ![Image](ArrayTests)
----------------------------------------------------------------------------------------------------------------------------------------------------------------

`FileExample.java`
  ![Image](FileExample)
----------------------------------------------------------------------------------------------------------------------------------------------------------------
`ListExamples.java`
![Image](linkedlist1)
![Image](linkedlist2)

----------------------------------------------------------------------------------------------------------------------------------------------------------------
`LinkedListExample.java`
![Image](list1)
![Image](list2)
![Image](list3)





