## Lab Report 2
## Test 1
## Part 1: Screenshot of code change


<img width="414" alt="image" src="https://user-images.githubusercontent.com/65454241/166863248-83193c09-72ff-418f-a443-1dadd8f3761c.png">




## Part 2: Link to test file for failure inducing input

[link for failure inducing input](breakin-test-lab2.md)


## Part 3: Symptom of failure inducing input

<img width="451" alt="image" src="https://user-images.githubusercontent.com/65454241/166863267-196d9317-a528-444a-9923-6235232e6c7e.png">


The error is that all of the links were not recognized.

## Part 4: Relationship between bug, symptom, and failure inducing input


The problem is that it would not recognize the 2nd type of link formatting in the breaking test file. It would only recognize the other type link. There would be a bug because we don’t get all of the output that we expect. So I modified the code in order to be able to collect the second type of link. !




## Test 2
## Part 1: Screenshot of code change

<img width="451" alt="image" src="https://user-images.githubusercontent.com/65454241/166863448-f1c1fd70-3fae-492c-9c76-4f6a58bd1bf2.png">



## Part 2: Link to test file for failure inducing input

[link for failure inducing input](test-file2.md)


## Part 3: Symptom of failure inducing input


<img width="451" alt="image" src="https://user-images.githubusercontent.com/65454241/166863476-2a6846a4-d9c0-4e18-abdc-345bb6be52c1.png">



## Part 4: Relationship between bug, symptom, and failure inducing input

The loop would not know when to stop. As a result, we would see an ‘OutOfMemoryError’ in the output. In order to fix this an extra condition must be added in the loop so that it knows when to stop. 



## Test 3
## Part 1: Screenshot of code change

<img width="451" alt="image" src="https://user-images.githubusercontent.com/65454241/166863677-7eb20536-d98f-4f7a-9e8b-b8d49ff82c50.png">


## Part 2: Link to test file for failure inducing input

[link for failure inducing input](breakin-test-lab2.md)


## Part 3: Symptom of failure inducing input


<img width="451" alt="image" src="https://user-images.githubusercontent.com/65454241/166863755-0eb1d1a3-a76f-4277-8e60-e3899538f538.png">



## Part 4: Relationship between bug, symptom, and failure inducing input

The loop wouldn’t know when to stop and there would be a repetition as the method would run again. That is why I added an extra condition in the loop so that the second method (getlinks2) would know when to stop.

