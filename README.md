# Circulate-the-values-of-N-variables
## Aim:
To write a python program to circulate the n variables using function concept
## Equipment’s required:
PC
Anaconda - Python 3.7
## Algorithm: 
### Step 1: 
create a function 
### Step 2:
store last value in temporary variable and change the value to privious value in a list
### Step 3: 
Get the value from the user for the number of rotation
### Step 4: 
Using the slicing concept rotate the list

### Step 5: 
change the first value into a value which was stored in temporary variable
### Step 6: 
display the output
## Program:
```
def circulate(lst):
    temp = lst[-1]
    for i in range(len(lst)-1, 0, -1):
        lst[i] = lst[i-1]
    lst[0] = temp
    return lst
n = int(input("Enter number of elements: "))
values = []
for i in range(n):
    val = int(input(f"Enter value {i+1}: "))
    values.append(val)
print("Before circulation:", values)
result = circulate(values)
print("After circulation:", result)
```
## Output:
<img width="392" height="238" alt="image" src="https://github.com/user-attachments/assets/127b1db4-fd8f-4d1a-aaab-5261e4fc320a" />

## Result:
The above code runned successfully and also cirulate the n value in list exits successfully
