# Lab Report 3
## Chosen command: grep
First command: -i 

Example 1: 
``` 
[cs15lwi23ang@ieng6-202]:skill-demo1-data:409$ grep -i "baHaMas" results.txt 
written_2/travel_guides/berlitz2/Bahamas-History.txt
written_2/travel_guides/berlitz2/Bahamas-Intro.txt
written_2/travel_guides/berlitz2/Bahamas-WhatToDo.txt
written_2/travel_guides/berlitz2/Bahamas-WhereToGo.txt
```

Example 2: 
``` 
[cs15lwi23ang@ieng6-202]:skill-demo1-data:417$ grep -i "CALIFORNIA" results.txt 
written_2/travel_guides/berlitz2/California-History.txt
written_2/travel_guides/berlitz2/California-WhatToDo.txt
written_2/travel_guides/berlitz2/California-WhereToGo.txt
``` 
What the -i command does for grep is search up a string without considering if the string is uppercase or lowercase. In the first example, 
I purposefully misspelled Bahamas and still got the files with "Bahamas" in the file name. Similarly, I used all capital letters to spell 
California and got my desired output regardless of capitals. 

--- 

Second command: -o

Example 1: 

```
[cs15lwi23ang@ieng6-202]:skill-demo1-data:418$ grep -o "Bahamas" results.txt 
Bahamas
Bahamas
Bahamas
Bahamas
``` 

Example 2: 
```
[cs15lwi23ang@ieng6-202]:skill-demo1-data:421$ grep -o "land" results.txt 
land
land
land
land
land
``` 
As per shown, the -o command prints just the inputted String from the command and separates each occasion of the word on each line. 
In other words, it prints out each matched String on separated lines. In the first example I search for the specific String "Bahamas" 
and got prompted with few results. For my second example I search for the String "land" which similarly prints all instances of "land" on separated lines. 

--- 

Third command: -n 

Example 1:
```
[cs15lwi23ang@ieng6-202]:skill-demo1-data:422$ grep -n "Cuba" results.txt 
217:written_2/travel_guides/berlitz2/Cuba-History.txt
218:written_2/travel_guides/berlitz2/Cuba-WhatToDo.txt
219:written_2/travel_guides/berlitz2/Cuba-WhereToGo.txt
```

Example 2: 

```
[cs15lwi23ang@ieng6-202]:skill-demo1-data:426$ grep -n "Athens" results.txt 
167:written_2/travel_guides/berlitz2/Athens-History.txt
168:written_2/travel_guides/berlitz2/Athens-Intro.txt
169:written_2/travel_guides/berlitz2/Athens-WhatToDo.txt
170:written_2/travel_guides/berlitz2/Athens-WhereToGo.txt
``` 

The command -n is a more descriptive version of -o, in the way that it outputs all matched strings but additionally shows the line
of the file. As you can see from the example, the searches for "Cuba" and "Athens" prompt you with not only the lines that contain the desired 
string, but also prompts their line number at the beginning of each line. 

--- 

Fourth command: -c 

Example 1: 
``` 
[cs15lwi23ang@ieng6-202]:skill-demo1-data:431$ grep -c "Cuba" results.txt 
3
```

Example 2: 
```
[cs15lwi23ang@ieng6-202]:skill-demo1-data:432$ grep -c "History" results.txt 
46
```

The -c command prints the number of times the given String is found in the file name. For instance, for the string "Cuba", it is only found 
in 3 file names. On the other hand, searching for how many lines contain "History" prompts me with a higher number as the string "History"
is found in many file names. 

--- 
Resources used: https://www.geeksforgeeks.org/grep-command-in-unixlinux/ (used for all commands) 















