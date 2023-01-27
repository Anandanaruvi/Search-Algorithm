# Linear Search and Binary search

## Aim:

To write a program to perform linear search and binary search using python programming.

## Equipment’s required:

1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm:

## Linear Search:

1.	Start from the leftmost element of array[] and compare k with each element of array[] one by one.

2.	If k matches with an element in array[] , return the index.

3.	If k doesn’t match with any of elements in array[], return -1 or element not found.

## Binary Search:

1.	Set two pointers low and high at the lowest and the highest positions respectively.

2.	Find the middle element mid of the array ie. arr[(low + high)/2]

3.	If x == mid, then return mid.Else, compare the element to be searched with m.

4.	If x > mid, compare x with the middle element of the elements on the right side of mid. This is done by setting low to low = mid + 1.

5.	Else, compare x with the middle element of the elements on the left side of mid. This is done by setting high to high = mid - 1.

6.	Repeat steps 2 to 5 until low meets high

## Program:

i)	#Use a linear search method to match the item in a list.
```
def selection_sort(nums):
    for i in range(len(nums)):
        lowest_value_index=i
        for j in range(i+1,len(nums)):
            if nums[j]<nums[lowest_value_index]:
                lowest_value_index=j
        nums[i],nums[lowest_value_index]=nums[lowest_value_index],nums[i]
list_of_nums=eval(input())
selection_sort(list_of_nums)
print(list_of_nums)
    
    



```
ii)	# Find the element in a list using Binary Search(Iterative Method).
```
def selection_sort(nums):
    for i in range(len(nums)):
        lowest_value_index = i
        for j in range(i+1, len(nums)):
            if nums[j] < nums[lowest_value_index]:
                lowest_value_index = j
        nums[i], nums[lowest_value_index] = nums[lowest_value_index], nums[i]

list_of_nums = eval(input())
selection_sort(list_of_nums)
print(list_of_nums)




```
iii)	# Find the element in a list using Binary Search (recursive Method).
```
def insertion_sort(nums):

    for i in range(1, len(nums)):

        item_to_insert = nums[i]

        j = i - 1

        while j >= 0 and nums[j] > item_to_insert:

            nums[j+1] = nums[j]

            j -= 1

        nums[j+1] = item_to_insert

        

list_of_nums = eval(input())

insertion_sort(list_of_nums)




```
## Sample Input and Output

![](./selection1.png)
![](./selection2.png)

## Result

Thus the linear search and binary search algorithm is implemented using python programming.