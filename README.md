# new-test

this is my test repo

arr = []
for v in range(4):
    arr.append(int(input("Enter number: ")))
print(arr)

x = int(input("Enter the search value: "))

def BINARYSEARCH(arr,low,high,x):
    if high >= low:
        mid = (high + low)//2
        if arr[mid] == x:
            return mid
        elif arr[mid]<x :
            return BINARYSEARCH(arr,mid+1,high,x)
        elif arr[mid]>x:
            return BINARYSEARCH(arr,low,mid-1,x)
    else:
        return -1

print(str(BINARYSEARCH(arr,0,len(arr)-1,x)))
