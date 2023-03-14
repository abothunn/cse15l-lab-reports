# Lab Report 5: 

Favorite Lab Report Chosen: Lab Report 3 

## Exploring command: grep -i

What it does: Basically takes in a string to search up, but this time, ignores all lowercase and uppercase characters, allowing you to have broader search 
results when finding your desired word.

Examples: 
```
[cs15lwi23ang@ieng6-202]:skill-demo1-data:409$ grep -i "BAHamaS" results.txt 
written_2/travel_guides/berlitz2/Bahamas-History.txt
written_2/travel_guides/berlitz2/Bahamas-Intro.txt
written_2/travel_guides/berlitz2/Bahamas-WhatToDo.txt
written_2/travel_guides/berlitz2/Bahamas-WhereToGo.txt
```
and 

```
[cs15lwi23ang@ieng6-202]:skill-demo1-data:417$ grep -i "CALifORNIA" results.txt 
written_2/travel_guides/berlitz2/California-History.txt
written_2/travel_guides/berlitz2/California-WhatToDo.txt
written_2/travel_guides/berlitz2/California-WhereToGo.txt
```
---

Another grep command that I like more than the others was: grep -c

The reason I liked this command was because of its convenience at simplicity. What the command does is search up all instances of desired 
string, but rather than printing instaces on all lines, it just prints the number of instances of where it found the exact string that was inputted.

Examples: 

```
[cs15lwi23ang@ieng6-202]:skill-demo1-data:431$ grep -c "Cuba" results.txt 
3
```
also, 
```
[cs15lwi23ang@ieng6-202]:skill-demo1-data:432$ grep -c "History" results.txt 
46
``` 

The uses for this command can be used very widely with some slight convenience, given that it returns only one line. 
