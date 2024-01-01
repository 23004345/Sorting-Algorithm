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

def selection_sort(nums):

    for i  in range(len(nums)):
    
        lowest_value_index=i
        
        for j in range(i+1,len(nums)):
        
            if nums[j]<nums[lowest_value_index]:
            
                lowest_value_index=j
                
        nums[i],nums[lowest_value_index] = nums[lowest_value_index],nums[i]  
        
    
    
list_of_nums = eval(input())

selection_sort(list_of_nums)

print(list_of_nums)

ii)	#Insertion Sort

def insertion_sort(nums):

    for i in range(1,len(nums)):
    
        item_to_insert=nums[i]
        
        j=i-1
        
        while j>=0 and nums[j] > item_to_insert:
        
            nums[j+1]=nums[j]
            
            j-=1
            
            nums[j+1]=item_to_insert
            
    
      
list_of_nums = eval(input())

insertion_sort(list_of_nums)

print(list_of_nums)



## Output:
i)	#Selection Sort
![Screenshot 2024-01-01 122452](https://github.com/23004345/Sorting-Algorithm/assets/138849203/86f4d77f-ebd9-4a3e-a737-9996c4e8c729)

ii)	#Insertion Sort
![Screenshot 2024-01-01 122506](https://github.com/23004345/Sorting-Algorithm/assets/138849203/81df9f62-f8a8-4231-800e-19cd45f78f20)


## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
