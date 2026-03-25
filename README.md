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
# Register No: 212225240141
# Developed By: SATHEESWARI.S
# 1-Norm of a Matrix

import numpy as np
def find_1_norm(matrix_data):
    matrix = np.array(matrix_data)
    norm_1 = np.linalg.norm(matrix, ord=1)
    print(f"{norm_1:.2f}")
input_matrix = [[-1, 3], [3, -4], [1, 7]]
find_1_norm(input_matrix)


# 2-Norm of a Matrix
import numpy as np

def calculate_l2_norm(matrix_data):
    matrix = np.array(matrix_data)
    l2_norm = np.linalg.norm(matrix, ord=2)
    return "{:.2f}".format(l2_norm)
test_1 = [[1, 2], [3, 4]]
test_2 = [[-1, 3], [3, -4], [1, 7]]
print(f"Input: {test_1} -> Result: {calculate_l2_norm(test_1)}")
print(f"Input: {test_2} -> Result: {calculate_l2_norm(test_2)}")



# Infinity Norm of a Matrix

import numpy as np
def matrix_infinity_norm(matrix_data):
    matrix = np.array(matrix_data)
    result = np.linalg.norm(matrix, ord=np.inf)
    return "{:.2f}".format(result)
input_data = [[-1, 3], [3, -4], [1, 7]]
print(matrix_infinity_norm(input_data)) 




```
## Output:
### 1-Norm of a Matrix
<img width="794" height="533" alt="Screenshot 2026-03-25 111452" src="https://github.com/user-attachments/assets/69830a07-396c-4ae7-8c7c-83818668e02a" />


### 2-Norm of a Matrix
<img width="1155" height="770" alt="Screenshot 2026-03-25 111211" src="https://github.com/user-attachments/assets/f357731f-f4f3-42b9-bbab-b250da543b17" />


### Infinity Norm of a Matrix

<img width="813" height="570" alt="Screenshot 2026-03-25 111233" src="https://github.com/user-attachments/assets/9e097afa-c1af-4e1f-8889-b9a205fefb7d" />

## Result
Thus the program for 1-norm, 2-norm and Infinity norm of a matrix are written and verified.
