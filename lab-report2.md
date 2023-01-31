# Lab Report 2 - Servers and Bugs (Week 3)

## Part 1
![Image](lab3_3.png)

![Image](lab3_1.png)
![Image](lab3_2.png)


* Which methods in your code are called?
handleRequest

* What are the relevant arguments to those methods, and the values of any relevant fields of the class?

* How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why.


## Part 2
Debug for ArrayMethods

A failure-inducing input for the buggy program, as a JUnit test and any associated code (write it as a code block in Markdown)
```@Test
  public void testaverageWithoutLowest() {
    double[] input1 = { };
    assertEquals(0.0, ArrayExamples.averageWithoutLowest(input1), 0.01);

    double[] input2 = {1.0, 2.0, 3.0, 4.0};
    assertEquals(3.0, ArrayExamples.averageWithoutLowest(input2), 0.01);
  }```

An input that doesn’t induce a failure, as a JUnit test and any associated code (write it as a code block in Markdown)

The symptom, as the output of running the tests (provide it as a screenshot of running JUnit with at least the two inputs above)

The bug, as the before-and-after code change required to fix it (as two code blocks in Markdown)

