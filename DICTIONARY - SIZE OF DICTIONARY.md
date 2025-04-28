# Exp.No:16  
## DICTIONARY - Write a program to get the maximum and minimum value of dictionary.Hint dict1 = {‘key 1’: 200, ‘key 2’: 300} Expected output Max: 300 Min: 200

### AIM  
To find the maximum and minimum values from a given dictionary and print them.

### ALGORITHM

1.Define the dictionary dict1 containing key-value pairs.

2.Use the values() method of the dictionary to get the list of values.

3.Find the maximum value using the max() function.

4.Find the minimum value using the min() function.

5.Print the maximum and minimum values.



### PROGRAM

```
#Reg.No:212223020020
#Name:Pradaksha V
dict1 = {'key 1': 200, 'key 2': 300}
val = dict1.values()
max = max(val)
min = min(val)

print(f"{max} is maximum")
print(f"{min} is minimum")

```

### OUTPUT

![image](https://github.com/user-attachments/assets/bb672f37-54de-48bc-91fd-3c52be7690d0)


### RESULT
The program successfully finds and prints the maximum and minimum values from the dictionary. For the dictionary {'key 1': 200, 'key 2': 300}, the output will be:
Max: 300
Min: 200
