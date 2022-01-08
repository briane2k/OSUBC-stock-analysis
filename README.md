# Analysis of Green-Stocks-Analysis Code Refactoring

 ### This Analysis is to see if refactoring the code summarizing the Green Stocks dataset improves its performace, as measured by run time.
  
  Although some varience was observed in repeated run times between Old Code to Old Code, and Refactored Code to Refactored Code, this is not in the scope of this analysis, it may however be due to available resources of the PC the Code was run on.
Ignoring this it is still evident that this Example of Code refactoring does positivly impact code performance.

See Image 
![Old Code 2017.png](/Resources/Old%20Code%202017.png)![VBA_Challenge_2017.png](/Resources/VBA_Challenge_2017.png)

You can see Old code 2017 (0.9609375)  <<-->>  Refactored code 2017 (0.1015625)

  thats x9.462 LESS time.

and
![Old Code 2018.png](/Resources/Old%20Code%202018.png)![VBA_Challenge_2018.png](/Resources/VBA_Challenge_2018.png)

Again Old code 2018 (1.132813)  <<-->>  Refactored code 2018 (0.109375)	

  with a x10.357 LESS time.



 ###  I believe this indicates refactoring was successfull.
The most concise explaination is (see attached images of code snippets)Old Code Nested Loop 12x3012.png   new code simply one Loop 12.png

![Old_Code_Nested_Loop_12x3012.png](/Resources/Old_Code_Nested_Loop_12x3012.png)

![new_code_simply_one_Loop_12.png](/Resources/new_code_simply_one_Loop_12.png)

The old code had 2 loops, one nested in the 2nd, the first loop had 12 elements, and the inside loop had 3012, for a total of 36,144

the new code has just 3,012
There is very little difference between the 2017 metrics and the 2018 metrics.

 ### There are advantages to refactoring code.
 These can be faster run times, as in our case, or lower space requirements, like for example using fewer variables in situation that uses many per data item.
Some situations, however refactoring might not help, it may occur that more time is spent refactoring, than is saved, or the even if refactoring is easy, the improvments in run time might be so negligable, it does not matter.  
However even if it doesn't seem like refactoring would improve run time, it must be kept in mind potential scale up in the future. A small difference in 3,000 data items isnt much, but if there were 3,000,000 dataitems it would quickly become worth it to refactor.
Code refactoring can also be used to make code more readable, which can decrease the effort required to maintain a codebase.
 ## Concluding, in our case the code refactor speed up runtimes by about 90%, made the code a little more concise, and didnt take prohibitive amounts of effort.
It was worth the effort in my opinion.
