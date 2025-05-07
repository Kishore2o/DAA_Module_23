# EX 5C Kadane's Algorithm
## DATE:
## AIM:
To write a python program to find the maximum contiguous subarray.


## Algorithm
1. 
2. 
3. 
4.  
5.   

## Program:

Developed by: Kishore S
Register Number:  212222240050
```python
def maxSubArraySum(a,size):
    max_till_now = a[0]
    max_ending = 0
    for i in range(0, size):
        max_ending = max_ending + a[i]
        if max_ending < 0:
            max_ending = 0
        elif (max_till_now < max_ending):
            max_till_now = max_ending
    return max_till_now
n=int(input())  
a =[] #[-2, -3, 4, -1, -2, 1, 5, -3]
for i in range(n):
    a.append(int(input()))
print("Maximum contiguous sum is", maxSubArraySum(a,n))
```

## Output:
![image](https://github.com/user-attachments/assets/9100c465-2221-49e6-82e3-44d85d36afbb)



## Result:
Thus the program was executed successfully for finding the maximum contiguous sum of subarray..
