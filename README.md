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
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by: Abishai K C
RegisterNumber: 23001564
'''
def selection_sort(nums):
    for i in range(len(nums)):
        mini = i
        for j in range(i+1,len(nums)):
            if nums[mini] > nums[j]:
                mini = j
        nums[i],nums[mini] = nums[mini],nums[i]
    return nums
list_of_nums = eval(input())
print(selection_sort(list_of_nums))

```
ii)	#Insertion Sort
```
''' 
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by: Abishai K C
RegisterNumber: 23001564
'''
def insertion_sort(nums):
    for i in range(len(nums)):
        curr = nums[i]
        j = i-1
        while j>=0 and nums[j]>curr:
            nums[j+1] = nums[j]
            j-=1
        nums[j+1] = curr
    return nums
list_of_nums = eval(input())
value = insertion_sort(list_of_nums)
print(value)

```

## Output:
## Selection Sort
![insertion](https://github.com/Abishai95141/Sorting-Algorithm/assets/139335314/133120d1-9b1c-4f69-896d-f272ccc9c068)
## Insertion Sort
![selection](https://github.com/Abishai95141/Sorting-Algorithm/assets/139335314/e56637c3-9296-4810-883b-88fc20e0b2a3)

## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
