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
```def linearSearch(array,n,k):
    for i in range(0,n):
        if array[i]==k:
            print("Element found at index: ",i)
            break
    else:
        print("Element not found ")
array=eval(input())
array.sort()
print(array)
k=int(input())
n=len(array)
result=linearSearch(array,n,k)



```
ii)	# Find the element in a list using Binary Search(Iterative Method).
```
def BinarySearch(array, k, low, high):
    while(low<=high):
        m=(low+high)//2
        if k==array[m]:
            return m
        elif k>array[m]:
            low=m+1
        else:
            high=m-1
    else:
        return -1
array=eval(input())
array.sort()
print(array)
k=eval(input())
n=len(array)
t=BinarySearch(array, k, 0, n-1)
if t==-1:
   print("Element not found")
else:
    print("Element found at index: ",t)




```
iii)	# Find the element in a list using Binary Search (recursive Method).
```
ef BinarySearch(arr, k, low, high):
    if high>=low:
        mid=low+(high-low)//2
        if arr[mid]==k:
            return mid
        elif arr[mid]>k:
            return BinarySearch(arr,k,low,mid-1)
        else:
            return BinarySearch(arr,k,mid+1,high)
    else:
        return -1
arr = eval(input())
arr.sort()
k = eval(input())
result=BinarySearch(arr,k,0,len(arr)-1)
if(result ==-1):
    print(arr)
    print("Element not found")
else:
    print(arr)
    print("Element found at index: ",result)





```
## Sample Input and Output

![WhatsApp Image 2023-12-30 at 22 10 06_d7e86ed6](https://github.com/ibrahimfedahs/Search-Algorithm/assets/150319493/72bd3998-9f44-4225-9389-918aac80d342) 
![WhatsApp Image 2023-12-30 at 22 10 33_82030483](https://github.com/ibrahimfedahs/Search-Algorithm/assets/150319493/9bb8e7aa-4c78-4578-af3f-2ed6e81f1b6b)
![WhatsApp Image 2023-12-30 at 22 11 14_0d9393b8](https://github.com/ibrahimfedahs/Search-Algorithm/assets/150319493/d4d3d982-e451-4ee0-b030-7bb2862e89f3)




## Result
Thus the linear search and binary search algorithm is implemented using python programming.
