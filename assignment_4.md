***Course :** python |
**Module :** Advanced*

### **Question 1 :** *Write a function that takes an exploder function and N. the exploder function explodes the given string into N times*
 *Function Prototype:*
```
  Exploder(string,n)
  Myfun(string,exploder,n)
```

 **Input:** guvi 5
 
 **Output:** guviguviguviguviguvi 
 
```python
def Exploder(string,n):
    return string*n
def Myfun(string,Exploder,n):
    print(Exploder(string,n))
string,n=input().split()
n=int(n)
Myfun(string,Exploder,n)
```

### **Question 2 :** *Display fibonacci series, and store the values in a List*

```python
n=int(input())
n1,n2=0,1
count=0
if n==1:
  print(n1)
else:
  while count < n :
    print(n1)
    temp = n1+n2
    n1=n2
    n2=temp
    count+=1
```

### **Question 3 :** *Jarvis has a list of names and he wants to convert the list items into uppercase. Write a function that takes list and converts all the items in the list to upper*

**PS:** *Use list comprehension to solve this*

```python
l=[i for i in input().split()]
li=[x.upper() for x in l]
print(li)
```
