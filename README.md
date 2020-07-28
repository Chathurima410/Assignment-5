# Assignment-5
In [ ]:

[0,1,2,10,4,1,0,56,2,0,1,3,0,56,0,4] sort increasing order but all zeroes should be at right hand side.

In [ ]:
list1=[0,1,2,10,4,1,0,56,2,0,1,3,0,56,0,4]              #given list of integers
list1.sort()                      
list2=[0]
c=list1.count(0)
list2=list2*c
list1=[i for i in list1 if i != 0]
print("The sorted list:",list1+list2)
The sorted list: [1, 1, 1, 2, 2, 3, 4, 4, 10, 56, 56, 0, 0, 0, 0, 0]
list1=[10,20,40,60,70,80] sorted list ;list2=[5,15,25,35,45,60] sorted list. Merge these two sorted list products one sorted list.

In [2]:
list1=[10,20,40,60,70,80]
list2=[5,15,25,35,45,60]
list3=list1+list2
list4=[]
for i in range(0,len(list3)):
  list4.append(min(list3))
  list3.remove(min(list3))
print("The sorted list:",list4)
The sorted list: [5, 10, 15, 20, 25, 35, 40, 45, 60, 60, 70, 80]
