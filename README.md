# Python-program-to-Sort-first-half-in-ascending-order-and-second-half-in-descending-order-in-an-array

Sort First half in Ascending and Second half in descending order in Python
Here, in this page we will discuss the program to sort first half in ascending and second half in descending order in python programming language. We are given with an array and need to print the array in desired sorting way i.e, first half in increasing order and second half in descending order.

Here, in this page we will discuss two different methods to sort the given array such that it’s first half is in ascending order and second half in descending order.

Method 1 : Sort the entire array then, print first half in ascending and second half in descending.
Method 2 : Using alternative way of above method
Example
Input : arr[6] = [1, 90, 34, 89, 7, 9]
Output : 1 7 9 90 89 34
Method 1 (Sort using inbuilt sort function):
Sort the entire array using inbuilt sort function
Run a loop till first half and print the element.
Run a loop for second half and print the elements.
sort() function
The sort() method is a built-in Python method that, by default, sorts the list in ascending order.
However, you can modify the order from ascending to descending by specifying the sorting criteria.
sort the array in python
Related Pages
Calculate the sum of elements in an array

Reverse an Array

Sort the elements of an array

Finding the frequency of elements in an array

Sorting elements of an array by frequency

Method 1 : Code in Python
Run
# Python program to print first half in
# Python program to print first half in
# ascending order and the second half
# in descending order


# function to print half of the array in
# ascending order and the other half in
# descending order

def printOrder(arr,n) :
    # sorting the array
    arr.sort()
    
    # printing first half in ascending order
    i = 0
    while i < n/2: print(arr[i]) i=i+1 # printing second half in descending order j=n-1 while j >= n / 2 :
        print (arr[j])
        j = j - 1

# Driver code
arr = [5, 4, 6, 2, 1, 3, 8, 9, 7]
n = len(arr)

printOrder(arr, n)
Output
1 2 3 4  5 9 8 7 6 
Method 2 :
Sort the first half of the array in ascending order just because only the elements in the first half of the input array needs to be sorted in ascending order (In this way the original elements in the first half of the array will remain in the first half but in ascending order).
Sort the second half of the array in descending order just because only the elements in the second half of the input array needs to be sorted in descending order (In this way the original elements in the second half of the array will remain in the first half but in descending order)
Method 2 : Code in Python
Run
# Python 3 program to print first half
# in ascending order and the second half
# in descending order

# function to print half of the array in
# ascending order and the other half in
# descending order

def printOrder(arr, n):

    # sorting the array
    arr.sort()

    # printing first half in ascending order

    for i in range(n / 2):
        print(arr[i], end = " ")

    # printing second half in descending order

    for j in range(n - 1, n // 2 -1, -1) :
        print(arr[j], end = " ")

# Driver code
arr = [ 5, 4, 6, 2, 1, 3, 8, -1 ]
n = len(arr)
printOrder(arr, n)
Output
-1 1 2 3 8 6 5 4
