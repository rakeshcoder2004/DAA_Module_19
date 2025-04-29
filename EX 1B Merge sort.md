# EX 1B Merge Sort
## DATE:
## AIM:
To write a python program to sort the first half of the list using merge sort.

## Algorithm
1. If the array has more than one element, split it into two halves.
2.Recursively apply merge sort on both halves.
3.Compare elements of both halves and merge them into a sorted array.
4.Copy any remaining elements from the left or right half.
5.Return the fully sorted array.
   

## Program:
```
/*
Program to implement Merge Sort
Developed by: Rakesh V
Register Number:  212222110036
*/
```

```
def merge_sort(inp_arr):
    if len(inp_arr) > 1:
        mid = len(inp_arr) // 2  
        left_half = inp_arr[:mid]  
        right_half = inp_arr[mid:]  

        merge_sort(left_half)  
        merge_sort(right_half)  
        i = j = k = 0  
        while i < len(left_half) and j < len(right_half):
            if left_half[i] < right_half[j]:
                inp_arr[k] = left_half[i]
                i += 1
            else:
                inp_arr[k] = right_half[j]
                j += 1
            k += 1

        while i < len(left_half):
            inp_arr[k] = left_half[i]
            i += 1
            k += 1

        while j < len(right_half):
            inp_arr[k] = right_half[j]
            j += 1
            k += 1

inp_arr = []     
n = int(input())  
for i in range(n):
    inp_arr.append(int(input()))  

print("Input Array:\n")
print(inp_arr)

merge_sort(inp_arr)  

print("Sorted Array:\n")
print(inp_arr)
```

## Output:

![image](https://github.com/user-attachments/assets/f4fc51bc-aea9-41a5-83cd-2a3f0e746c2c)




## Result:
The program successfully sorts the first half of the given array using merge sort. where only the first half is sorted, and the second half remains unchanged.
