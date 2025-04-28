# Exp.No:17  
## EXCEPTION HANDLING:Place msg="You can't add int to string" to the right place so that program avoids BaseExceptionError.You can use except Exception although normally you should be careful using such powerful exception statements.

### AIM  
To handle the TypeError when attempting to add an integer to a string, and to print an appropriate error message instead of letting the program crash.

### ALGORITHM

1.Initialize a as a string ("Hello World!").

2.Attempt to add an integer (10) to the string.

3.If a TypeError occurs (since adding an integer to a string is not allowed), catch the exception.

4.Print a user-friendly message: "You can't add int to string".

5.End the program gracefully.

### PROGRAM

```
Reg.No:212223020020
Name:Pradaksha V
a="Hello World!"
try:
    a = a + 10
    print(a)
except TypeError:
    print("You can't add int to string")
```

### OUTPUT

![image](https://github.com/user-attachments/assets/fcb96807-9681-4cf0-acc6-a2e295cc02a0)

### RESULT
The program correctly catches the TypeError and prints the message: 'You can't add int to string', preventing the program from terminating unexpectedly.
