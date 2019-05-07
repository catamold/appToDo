---
title: Data Testing
parent: Iteration 1
has_children: false
---

## Data Testing
Testing process was implemented using NUnit which can be run from a console runner, within Visual Studio through a Test Adapter. It provides a rich set of assertions as static methods of the Assert class. If an assertion fails, the method call does not return and an error is reported. If a test contains multiple assertions, any that follow the one that failed will not be executed. All the methods implemented were tested using NUnit extension.
> Encryption Data Test
>
> Decryption Data Test
>
> Tasks Sorting Less Equal Current Date
>
> Tasks Sorting according to Priority
>
> Tasks Sorting More Current Date
>
> Tasks Sorting according to Keywords Input
>
> Tasks Sorting according to Tags Keywords Input
>
Some tests failed, because of the incorrect results. In order to follow the code, I used debugging techniques like breakpoints. You set breakpoints wherever you want to pause debugger execution, so that you can see the state of code variables. 

Another method of testing is using System diagnostics package, so that you show data from Debug on Output.
> e.g. Debug.WriteLine(test.value);
