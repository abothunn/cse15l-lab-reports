# Lab Report 2
## Part 1

Code for `StringServer`:

![Image](StringServer.png)


First screenshot using `/add-message`: 
![Image](favoriteGame.png)

Description: The methods called in StringServer.java are the `URLHandler` method and the `main` method. The relevant argument for `URLHandler` is a URI String that takes in an  `url` string as a parameter which runs through "if statements" that check for relevant fields which are specific elements in the inputted url and the `stringVar` String variable. The relevant fields that do change only when the method is ran successfully is the `stringVar` variable that gets updated and returned. For further clarification, the `URLHandler` method is properly used when the user enters a valid url, which will update and return `stringVar`, thus displaying the message on the server screen and adds all subsequent url inputs inputted from the user. As for the `main` method, this method uses a `port number` created by the user to then host a local server. The relevant fields for main remain the same throughout the whole time the server is up. The host can turn off the server in which the port, an int, number is able to changed.

---
Second screenshot using `/add-message`:
![Image](awesomeJoe.png)

Description: In similar fashion as the last description, methods used are the `URLHandler` and the `main` method. For `URLHandler`, the relevant arguments are the inputted `url`s from the user. The relevant arugments change upon additional url inputs from the user, which all display on the server's screen. On the other hand, the `main` method is to be called allong with a four digit port number which hosts a local server that displays the url inputted from `URLHandler`. 

---

## Part 2

Bug Chosen: ReverseInPlace

Failure inducing input:
```
@Test
public void testReverseInPlace(){
int[] input = {1, 2, 3, 4, 5};
ArrayExamples.reverseInPlace(input);
assertArrayEquals(new int[]{5 , 4, 3, 2, 1}, input);
}
```

Non-failure inducing input: 
```
@Test
public void testReverseInPlace1(){
int[] input1 = {1, 1, 1, 1, 1};
ArrayExamples.reverseInPlace(input1);
assertArrayEquals(new int[]{1, 1, 1, 1, 1}, input1);
}
```

Failed case screenshot:
![Image](failedCase.png)




Passed case screenshot:
![Image](passedCase.png)


Bugged code: 
```
static void reverseInPlace(int[] arr) {
  for(int i = 0; i < arr.length; i += 1) {
    arr[i] = arr[arr.length - i - 1];
  }
}
```

Working code:
```
static void reverseInPlace(int[] arr) {
  int temp = 0;
  for(int i = 0; i < arr.length/2; i += 1) {
    temp = arr[i];
    arr[i] = arr[arr.length - i - 1];
    arr[arr.length - i - 1] = temp;
  }
}
```



The bug fix was essesntially making a temporary array that stores of the current index of the array in the loop. The temp array's values are then updated onto the new array, preventing the method from copying over an alread-updated array. If there were no temporary array, the reverse method would be trying to reverse the same array it's updating from, which causes in a wrong output. 
 
--- 

## Part 3

Something I've learned from week 2 and 3 that I didn't know before was testing with JUnit. I find it extremely convenient to be able to make specific test case scenarios to be able to pinpoint errors in my code. Creating test cases is a skill I look forward to utilizing in the future to aid me in my coding. Additionally, I didn't know it was possible to create a local server from java and be able to access the server in the browser through the use of a port number. 

