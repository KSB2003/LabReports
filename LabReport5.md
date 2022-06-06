## Lab Report 5

 - How you found the tests with different results (Did you use vimdiff on the
results of running a bash for loop? Did you search through manually? Did you
use some other programmatic idea?)

     Answer: I searched through manually for both test cases. 

## Test 1: 495

## Describe which implementation is correct, or neither if both give the wrong output:
 - My group's implementation is wrong and the provided implementation is correct.


## Provide a link to the test-file with different-results (in the provided repository or your repository , either is fine)

[test-495](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/495.md)



## Indicate both actual outputs (provide screenshots) and also what the expected output is (list the links that are expected in the output).

Output of provided implementation:

`[foo(and(bar))]`

Output of group/my implementation:

`[foo(and(bar]`

Expected output:

`[foo(and(bar))]`


## Bug description and fix

The highlighted line in the error is the error in the code. It matches the first open with the first closed bracket and it fails to stack additional brackets. In order to fix this I would implement a stack program to find the matching brackets. 


<img width="394" alt="Screen Shot 2022-06-05 at 6 01 42 PM" src="https://user-images.githubusercontent.com/65454241/172078700-74eab534-0ba8-43c6-80ee-dfeab85e9dad.png">


## Test 2: 504
## Describe which implementation is correct, or neither if both give the wrong output:
 - Both of the implementations are incorrect, both mine and the given implementation.
    - The wrong output given by my implemenation was as follows `[/url "title", /url 'title', /url (title]`.
    - The wrong output given by the given implemenation was as follows `[]`.




## Provide a link to the test-file with different-results (in the provided repository or your repository , either is fine)


[test-504](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/504.md)



## Indicate both actual outputs (provide screenshots) and also what the expected output is (list the links that are expected in the output).

Output of provided implementation:

`[]`

Output of group/my implementation:

`[/url "title", /url 'title', /url (title]`


Expected output:

`[/url "title", /url 'title', /url (title)]`


## Bug description and fix

The highlighted line in the error is the error in the code. It matches the first open with the first closed bracket and it fails to include the closed bracket of the last entry. In order to fix this we can add an extra if condition that would help include the final closing parenthesis. 


<img width="371" alt="Screen Shot 2022-06-05 at 6 42 25 PM" src="https://user-images.githubusercontent.com/65454241/172081149-514e4bd3-0a7f-4818-b3d7-819787e199e2.png">
