## Stack-Stack Reversal Program 🔁

This Python program demonstrates how to reverse the values in a stack using basic stack operations like push and pop.

## 🎯 Aim

To write a Python program that reverses the values in a stack using standard stack operations.

## 📋 Algorithm

1. Create an empty stack.
2. Read an integer `n` from the user (number of elements to push).
3. Loop `n` times:
   - Read an integer from the user.
   - Push it onto the stack.
4. Create an empty list called `reverse`.
5. While the stack is not empty:
   - Pop the top element.
   - Append it to `reverse`.
6. Print the reversed list.


### Program:
```
def insertAtBottom(s, item):
    if not s:
        s.append(item)
        return
    top = s.pop()
    insertAtBottom(s, item)
    s.append(top)

def reverseStack(s):
 
    if not s:
        return
 
    item = s.pop()
    reverseStack(s)
 
    insertAtBottom(s, item)
    return s
l=[]
n=int(input())
for i in range(n):
    l.append(int(input()))
print(reverseStack(l))
```

## 🧪 Sample Input and Output
<img width="513" height="277" alt="image" src="https://github.com/user-attachments/assets/f8ec8d8f-7a46-40b3-82ea-9cc0a087c2b4" />

## Result
Thus,the program is executed successfully

