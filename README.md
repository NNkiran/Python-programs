# Python-programs

def reverse_an_array(arr):
    #using two pointer method we can solve this problem p1 is first pointer and p2 is second pointer 
    #first pointer is placed ar index postion '0' and last pointer pointer fix at end of the array means last element 
    p1 = 0
    p2 = len(arr)-1
    while(p1<p2):
        # p1 = p1 + p2
        # p2 = p1 - p2
        # p1 = p1 - p2
        temp = arr[p1]
        arr[p1] = arr[p2]
        arr[p2] = temp
        p1 += 1
        p2 -= 1
    return arr
    

arr=[2,4,6,8,10,12,14]
print(reverse_an_array(arr)) 


def is_Sorted(arr):
    for i in range(1,len(arr)):
        if(arr[i] < arr[i-1]):
            return False
    return True
       
       
arr=[2,4,6,8,10,12,14]
print(is_Sorted(arr))
