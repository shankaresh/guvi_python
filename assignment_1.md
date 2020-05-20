***Course :** python |
**Module :** Beginner*


### **Question 1 :** *Print a given input*
```python
a=input()
print(a)
```

### **Question 2 :** *Given an array of integers ,add one to the last element in the array of integer*
```python
a=[1,[2,3],4,5]
a.append(6)
print(a)
```

### **Question 3 :** *Find the length of the last word from the given input string*
```python
a="To find last word's length "
x=a.strip()
l=0
for i in range(len(x)):
  if x[i] == " ":
    l=0
  else:
    l+=1
print(l)
```
