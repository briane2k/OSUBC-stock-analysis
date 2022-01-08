# Analysis of Green-Stocks-Analysis Code Refactoring

 ### This Analysis is to see if refactoring the code summarizing the Green Stocks dataset improves its performance, as measured by run time.
  
  Although some variance was observed in repeated run times between Old Code to Old Code, and Refactored Code to Refactored Code, this is not in the scope of this analysis, it may however be due to available resources of the PC the Code was run on.
Ignoring this it is still evident that this Example of Code refactoring does positively impact code performance.

See Image 
![Old Code 2017.png](/Resources/Old%20Code%202017.png)![VBA_Challenge_2017.png](/Resources/VBA_Challenge_2017.png)

You can see Old code 2017 (0.9609375)  <<-->>  Refactored code 2017 (0.1015625)

  thats roughly 89% faster.

and
![Old Code 2018.png](/Resources/Old%20Code%202018.png)![VBA_Challenge_2018.png](/Resources/VBA_Challenge_2018.png)

Again Old code 2018 (1.132813)  <<-->>  Refactored code 2018 (0.109375)	

  thats roughly 90% faster.



 ###  I believe this indicates refactoring was successful.
The most concise explanation is (see attached images of code snippets)Old Code Nested Loop 12x3012.png   new code simply one Loop 12.png

![Old_Code_Nested_Loop_12x3012.png](/Resources/Old_Code_Nested_Loop_12x3012.png)

![new_code_simply_one_Loop_12.png](/Resources/new_code_simply_one_Loop_12.png)

The old code had 2 loops(shown first), one nested in the 2nd, the first loop had 12 elements, and the inside loop had 3012, for a total of 36,144

the new code(shown 2nd) has just 3,012
There is very little difference between the 2017 metrics and the 2018 metrics.

 ### There are advantages to refactoring code.
 These advantages can include faster run times, as in our case, or lower space requirements, for example using fewer variables in a situation that uses many variables per data item(row).
However refactoring might not help, as it may take more time to refactor than is saved, or even if refactoring is easy, the improvements in run time might be so negligible, it would not be worth the time spent. However refactoring should be considered if there could be a large scale up in the future. A small difference in 3,000 data items is not much, but if there were 3,000,000 data items it would quickly become worth it to refactor.
Code refactoring can also be used to make code more readable, which can decrease the effort required to maintain a codebase.
 ## Concluding, in our case the code refactor sped up runtimes by about 90%, made the code a little more concise, and didn't take prohibitive amounts of time/effort.
It was worth the effort in my opinion.
