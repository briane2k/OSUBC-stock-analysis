Analysis of Green-Stocks-Analysis Code Refactoring
  This Analysis is to see if refactoring the code summarizing the Green Stocks dataset improves its performace, as measured by run time.
  Although some varience was observed in repeated run times between Old Code to Old Code, and Refactored Code to Refactored Code, this is not in the scope of this analysis, it may however be due to available resources of the PC the Code was run on.
Ignoring this it is still evident that this Example of Code refactoring does positivly impact code performance.
See Image 
	Old Code 2017.png(0.9609375)  <<-->>  VBA_Challenge_2017.png(0.1015625)   x 9.462 LESS
and
	Old Code 2018.png(1.132813)  <<-->>  VBA_Challenge_2018.png(0.109375)	x 10.357 LESS

I believe this indicates refactoring was successfull.
The most concise explaination is (see attached images)
<< Old Code Nested Loop 12x3012.png >>
<< new code simply one Loop 12.png >>

the old code had 2 loops, one nested in the 2nd, the first loop had 12 elements, and the inside loop had 3012, for a total of 36,144

the new code has just 3,012
There is very little difference between the 2017 metrics and the 2018 metrics.

  There are advantages to refactoring code, these can be faster run times, as in our case, or lower space requirements, like for example using fewer varialbes in situation that uses many per data item.
Some situations, however refactoring might not help, it may occur that more time is spent refactoring, than is saved, or the even if refactoring is easy, the improvments in run time might be so negligable, it does matter.  Additionaly, it must be kept in mind postential scale up in the future. A small difference in 3,000 data items isnt much, but if there were 3,000,000 dataitems it would quickly become worth it to refactor.
Code refactoring can also be used to make code more readable, which can decrease the effort required to maintain a codebase.
  In our case the code refactor speed up runtimes by about 90%, made the code a little more concise, and didnt take prohibitive amounts of effort.