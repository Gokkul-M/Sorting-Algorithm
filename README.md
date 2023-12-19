# Selection sort and Insertion sort
## Aim:
To write a program to perform selection sort and insertion sort using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Selection Sort Algorithm:
1.	Set the first unsorted element as the minimum
2.	For each of the unsorted elements, check if the element < current minimum.
3.	If yes, set the element as the new minimum.
4.	Swap minimum with first unsorted position.
5.	Repeat the steps 2 and 3 for all the elements in the array.
## Insertion Sort Algorithm:
1.	Set the first element as sorted element j.
2.	For each unsorted element X, check if current sorted element j >X.
3.	If yes, move sorted element to the right by 1.
4.	Break the loop and insert X.
5.	Repeat the steps 2 to 4 for sorting all the elements in the array.
## Program:
i)	#Selection Sort
```
''' 
# Program to sort the elements in the list using the Selection Sort algorithm.
Developed by: Gokkul M
RegisterNumber: 23014201
'''
def selection_sort(nums,size):
    for ind in range(size):
        min_index=ind
        for j in range(ind+1,size):
            if nums[j]<nums[min_index]:
                min_index=j
                (nums[ind],nums[min_index])=(nums[min_index],nums[ind])
arr=eval(input())
size=len(arr)
selection_sort(arr,size)
print(sorted(arr))
```
ii)	#Insertion Sort
```
''' 
# Program to sort the elements in the list using the Insertion Sort algorithm.
# Developed by: Gokkul M
# RegisterNumber:23014201 
'''
def insertion_sort(nums):
    n=len(nums)
    if n<=1:
        return
    for i in range(1,n):
        key=nums[i]
        j=i-1
        while j>=0 and key<nums[i]:
            nums[j+1]=nums[j]
            j=-1
nums=eval(input())
insertion_sort(nums)
print(sorted(nums))
```

## Output:
### i)	#Selection Sort
![image](https://github.com/Gokkul-M/Sorting-Algorithm/assets/144870543/41a6589c-101f-45aa-b4ce-4e10d1a36a18)
### ii)	#Insertion Sort
![image](https://github.com/Gokkul-M/Sorting-Algorithm/assets/144870543/6e37f299-2757-4bb7-93b1-6e1a3c232961)

## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
