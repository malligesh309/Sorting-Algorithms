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
```
Developed By: MALLIGESH M
Register No: 212223230074
```

i)	#Selection Sort


```
def selection_sort(arr):
    for i in range(len(arr)):
        min_index = i
        for j in range(i+1, len(arr)):
            if arr[j] < arr[min_index]:
                min_index = j

        arr[i], arr[min_index] = arr[min_index], arr[i]

    return arr


arr = eval(input())

sorted_arr = selection_sort(arr)
print(sorted_arr)

```
ii)	#Insertion Sort
```
def insertion_sort(arr):
    for i in range(1, len(arr)):
        key = arr[i]
        j = i - 1

        while j >= 0 and arr[j] > key:
            arr[j + 1] = arr[j]
            j -= 1

        arr[j + 1] = key

    return arr

arr = eval(input())  

sorted_arr = insertion_sort(arr)

print(sorted_arr)

```

## Output:
i)	#Selection Sort


![image](https://github.com/user-attachments/assets/b00b9acd-93fe-4f27-aee2-40724e3b43c9)

ii)	#Insertion Sort



![image](https://github.com/user-attachments/assets/4c2fa850-7999-4ccf-8e42-9b4460f10db8)


## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
