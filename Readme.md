##Author - Sankalp Verma
Topic - Rspec intro to the begineer level

---

##Different ways of testing code and Rspec config settings
Default left(global level, local level, cmd level)
1.To produce colour based output
--no-color --color

2.To produce documentation(-f p/d)
--format progress --format documentaion

3.Specify order, Randomized with seeds
--order defined --order random

4.Profile, tells information about the test(top 10 slow tests)
--no-profile --profile(-p)

5.Determine the way you want to solve failures, fail fast stops when finds a failure  
--no-fail-fast --fail-fast

6.If we want to run only one test, provide the line number after the filename
filename_spec.rb:line_number

---

##Pending and skipping Examples
Pending:-
1.omit the block
--Dont provide block to it/describe
2.use pending inside the block
--use pending("message") method in block, but make sure to provide failure code, as correct code will return error
--pending means some error is there and more work is left to be done on that code
--can be used for time consuming process

Skipping:-
1.use xdescribe or xit
--use x in front of it/describe and block will be skipped
2.use skip inside the block
--use skip("message") method to skip the content, default message is available.

---

##Rspec hierarchy
1.spec file ---> filename_spec.rb

2.example group ---> describe

3.nested group ---> describe/context

4.example ---> it

5.expectations ---> expect().to() OR expect().not_to()
