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

<img width="501" alt="Screen Shot 2022-04-24 at 7 24 33 PM" src="https://user-images.githubusercontent.com/65454241/165010528-ceececec-c067-46d1-a9a4-b7c62d9d9a88.png">

## Part 2: Link to test file for failure inducing input

[link for failure inducing input](breakin-test-lab2.md)


## Part 3: Symptom of failure inducing input

<img width="551" alt="Screen Shot 2022-04-24 at 7 02 32 PM" src="https://user-images.githubusercontent.com/65454241/165010652-031eabf0-699c-49d6-950b-3bc4fc1a628c.png">


## Part 4: Relationship between bug, symptom, and failure inducing input
The bug that I found was that I created two lists and I tried to add the elements from the second list into the first list but I made the mistake of just adding the elements from the second list to the second list instead of adding to the first list so I could get all of the links. The same symptom is there for all of the test cases.
