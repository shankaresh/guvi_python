***Course :** python |
**Module :** Intermediate*


### **Question 1 :** *Find the valid number from the given input string, if the given input string is valid print yes otherwise no*
```python
def is_valid_number(str): 
    i = 0
    j = len(str) - 1
    while i<len(str) and str[i] == ' ': 
        i += 1
    while j >= 0 and str[j] == ' ': 
        j -= 1
    if i > j: 
        return False 
    if (i == j and not(str[i] >= '0' and str[i] <= '9')): 
        return False
    if (str[i] != '.' and str[i] != '+' and 
        str[i] != '-' and not(str[i] >= '0' and 
        str[i] <= '9')): 
        return False
    flagDotOrE = False  
    for i in range(j + 1):          
        if (str[i] != 'e' and str[i] != '.' and 
            str[i] != '+' and str[i] != '-' and not
           (str[i] >= '0' and str[i] <= '9')): 
            return False
        if str[i] == '.': 
            if flagDotOrE: 
                return False
            if i + 1 > len(str): 
                return False
            if (not(str[i + 1] >= '0' and 
                    str[i + 1] <= '9')): 
                return False
        elif str[i] == 'e': 
            flagDotOrE = True
            if (not(str[i - 1] >= '0' and 
                    str[i - 1] <= '9')): 
                return False 
            if i + 1 > len(str): 
                return False 
            if (str[i + 1] != '+' and str[i + 1] != '-' and 
               (str[i + 1] >= '0' and str[i] <= '9')): 
                return False
    return True 
if __name__ == '__main__': 
    str = input()
    if is_valid_number(str): 
        print('yes') 
    else: 
        print('no') 
```

### **Question 2 :** *Print the length of the given input string*
```python
print(len(input()))
```

### **Question 3 :** *From the string Find the Number of occurence of letter r,if r doesnot occur print -1*
```python
a=input()
b=a.count('r') 
print(b if(b>0) else -1)
```
