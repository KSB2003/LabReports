## Lab Report 5

 - How you found the tests with different results (Did you use vimdiff on the
results of running a bash for loop? Did you search through manually? Did you
use some other programmatic idea?)

Answer: I searched through manually. 

## Test 1: 495

Describe which implementation is correct, or neither if both give the wrong output:
 - My group's implementation is wrong and the provided implementation is correct.

[link for test 495](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/495.md)

Output of provided implementation:
`[foo(and(bar))]`

Output of group/my implementation:
`[foo(and(bar]`

Expected output:
`[foo(and(bar))]`


The highlighted line in the error is the error in the code. It matches the first open with the first closed bracket and it fails to stack additional brackets. In order to fix this I would implement a stack program to find the matching brackets. 


<img width="394" alt="Screen Shot 2022-06-05 at 6 01 42 PM" src="https://user-images.githubusercontent.com/65454241/172078700-74eab534-0ba8-43c6-80ee-dfeab85e9dad.png">







