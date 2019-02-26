# Lazy Developer's Manifesto

## No code is the best code

The best code is the one which was never written. 
It has no bugs, it needs no maintenance, no code review, no testing, just nothing. 
It can’t break existing code and it does not break on software updates. 
It’s perfect. 
Whenever you can persuade your manager that the code is not needed - do that. 
The feature is not needed with a high probability. 
Moreover - delete the code which is not needed: dead code, commented out code, features which are not in use, flaky or forever ignored unit tests. 
The less code - the better. 
No code is the best.

## If you need code, try not to write it

Find out if the code has already been written for you. 
It can be in your code base but maybe it can be another library.  
Don’t fall into the trap of [Not Invented Here](https://en.wikipedia.org/wiki/Not_invented_here) syndrome. 
If you need to create an http or date handling library, think twice - probably someone has already written it. 
Spend some time learning the library and then just use it. 
There are bad libraries, but most of them are good enough.
If it’s an open source library and it has no feature you want it to have - contribute to it, it still will be faster than writing everything from scratch.
Anyway you will not write a better one with a high degree of probability.

## Write as much as you need but not more than that

If you say “What if I need it later” then later you write it. 
But most likely [you ain’t gonna need it](https://en.wikipedia.org/wiki/You_aren%27t_gonna_need_it).
If you still need to write code, [Keep It Simple, Stupid](https://en.wikipedia.org/wiki/KISS_principle). 
If your job should run every night - do a cron job. 
Don’t make it configurable with a property file or environment variable. 
Don’t deploy a separate server, don’t create a DB to store configuration in it, don’t create a REST and SOAP endpoints to change the configuration, don’t create a GUI with authorization and authentication with different permissions for different users, which implies another storage for user’s identity and yet another GUI to manage them. 
Don’t fall into a trap of creating an [Inner Platform](https://thedailywtf.com/articles/The_Inner-Platform_Effect) and don’t write a framework to handle different kinds of different jobs in different intervals if you only need to run this one single job. 
Cron job is enough. 
[Entities must not be multiplied beyond necessity](https://en.wikipedia.org/wiki/Occam%27s_razor).

## Don’t rewrite working code

[If it works, don’t touch it](https://en.wikipedia.org/wiki/Bert_Lance). 
And remember - one of the greatest sins is a [full rewrite](https://www.joelonsoftware.com/2000/04/06/things-you-should-never-do-part-i/).

## Find a simpler way

If a task seems too tedious, probably there is a simpler way. 
Find out - it may save you tons of time. 
If you have to write the same statement thousand times, maybe you don’t need to copy-paste. 
You may ask someone and they will tell you about the loops. 
On the other hand if the task is so hard that you can’t do it, maybe it’s impossible in a current setting. 
Find out the limitations - and then maybe you will have to write no code.

## Don’t strive for perfection

Perfect code might become obsolete by the time you finish it. 
Better done than perfect. 
[Worse is better](https://en.wikipedia.org/wiki/Worse_is_better). 
Don’t spend too much time thinking either. 
If it’s not about architecture and there are seemingly similar approaches, libraries, technologies, formats, tools each with its pros and cons, just pick any. 
[You can refactor it later](https://techblog.bozho.net/do-it-either-way-well-refactor-it-later/).

## Search engine is your friend 

If you can’t find the solution yourself, [search](https://www.google.com) for it. 
It would be called cheating at school. 
It is normal at work. 
You don’t have to invent solutions if the solutions are already [available](https://stackoverflow.com/).

## Automate everything

Many things you do can be automated through scripts. 
Let the scripts do the job for you. 
Writing some of the code can be automated as well. 
So let the tools do the job for you as well. 
Know what they can do. 
Make use of the editor of your choice - it may contains features to generate and manipulate code so that you dont have to do that yourself. 
Code generation tools do exist.

## Don’t hurry
Haste makes waste. 
This applies to code as well. 
If you write the code in haste, you introduce more bugs, you make it harder to read and you will spend more time later fixing the bugs and trying to understand what you wrote there than if you wrote it calmly in the first place.

