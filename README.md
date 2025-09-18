# Norm of a matrix
## Aim
To write a program to find the 1-norm, 2-norm and infinity norm of the matrix and display the result in two decimal places.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
	1. Get the input matrix using np.array()   
    2. Find the 2-norm of the matrix using np.linalg.norm()
	3. Print the norm of the matrix in two decimal places.
## Program:
```Python
# Register No: 212224230095
# Developed By: Infant Maria Stefanie .F
# 1-Norm of a Matrix

import numpy as np
mat = np.array(eval(input()))
ans = np.linalg.norm(mat,1)
Norm_of_matrix = "{:.2f}".format(ans)
print(Norm_of_matrix)

# 2-Norm of a Matrix

import numpy as np
mat = np.array(eval(input()))
ans = np.linalg.norm(mat,2)

Norm_of_matrix = "{:.2f}".format(ans)
print(Norm_of_matrix)

# Infinity Norm of a Matrix

def infinity_norm(matrix):
    row_sums=[sum(abs(x) for x in row) for row in matrix]
    return max(row_sums)
    
matrix=eval(input())
result=infinity_norm(matrix)
print(f"{result:.2f}")

```
## Output:
### 1-Norm of a Matrix

<img width="1458" height="310" alt="image" src="https://github.com/user-attachments/assets/a5661671-f746-44b3-9916-0a9822ad6256" />

<img width="1861" height="1039" alt="image" src="https://github.com/user-attachments/assets/c8466761-2fb2-4fd5-b02b-531e93170141" />

### 2-Norm of a Matrix

<img width="1881" height="1023" alt="image" src="https://github.com/user-attachments/assets/b570b110-5467-4f49-808c-570c0529ec95" />

<img width="1518" height="432" alt="image" src="https://github.com/user-attachments/assets/e388e6dd-6d10-46ab-a097-60e8bd92321e" />

### Infinity Norm of a Matrix

<img width="1853" height="1027" alt="image" src="https://github.com/user-attachments/assets/d22975d5-8047-4223-b70d-319de4f2831b" />

## Result
Thus the program for 1-norm, 2-norm and Infinity norm of a matrix are written and verified.
