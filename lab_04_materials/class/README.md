# Lab 04 - SOP/POS and KMaps

In this lab, you’ve learned how to apply KMaps, Sum Of Products and Products of
sums to simplify digital logic equations. Then, you’ve proven out that they work
using an implemented design on your Basys3 boards.

## Rubric

| Item | Description | Value |
| ---- | ----------- | ----- |
| Summary Answers | Your writings about what you learned in this lab. | 25% |
| Question 1 | Your answers to the question | 25% |
| Question 2 | Your answers to the question | 25% |
| Question 3 | Your answers to the question | 25% |

## Lab Summary

We used KMAPs to determine the min and max terms. Then we developed POS and SOP using the terms. From there we created the naive file which implemented all the cases where the output equals one. We implemented the POS and SOP into the corresponding files, ran the simulation and passed all the test cases. This allowed us to connect a Basys3 board to test our logic.  

## Lab Questions

### Why are the groups of 1’s (or 0’s) that we select in the KMap able to go across edges?
- logically they are connected because the KMAP is built like a cylinder where the edges are touching.

### Why are the names Sum of Products and Products of Sums?
- When finding the min terms you connect the inputs with AND gates and the groups of inputs are then connected with OR gates therefore creating a sum of products. Where are the max terms, inputs are connected via OR gates and the groups are connected with AND gates creating the product of sums.

### Open the test.v file – how are we able to check that the signals match using XOR?
- in the test.v file, there are if statements that verify if two leds have the same input, the result is 0 because of the logic of XOR. Therefore the XOR gate logic verifies if the signals are matching or not. If min or max terms match, the program is succesful.

