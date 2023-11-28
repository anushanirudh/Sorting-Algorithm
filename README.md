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
def selection_sort(nums):
    for i in range(len(nums)):
        low_index=i
        for j in range(i+1,len(nums)):
            if nums[j]<nums[low_index]:
                low_index=j
        nums[i],nums[low_index]=nums[low_index],nums[i]
    return nums
    
list_of_nums = eval(input())
values=selection_sort(list_of_nums)
print(values)





```
ii)	#Insertion Sort
```def insertion_sort(nums):
    for i in range(1,len(nums)):
        item=nums[i]
        j=i-1
        while j>=0 and nums[j]>item:
            nums[j+1]=nums[j]
            j-=1
        nums[j+1]=item
    return nums
    
list_of_nums = eval(input())
value=insertion_sort(list_of_nums)
print(value)






```

## Output:
i) #Selection Sort


![Screenshot (16)](https://github.com/anushanirudh/Sorting-Algorithm/assets/151725737/a33513b6-3ceb-4984-80a4-e33cc7258602)

ii) #Insertion Sort


![Screenshot (17)](https://github.com/anushanirudh/Sorting-Algorithm/assets/151725737/95d3b761-ead8-4aa2-a1d8-dbaa0434f094)



## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
