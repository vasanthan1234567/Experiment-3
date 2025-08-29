# Experiment-3
## PRIME NUMBER OR NOT
### Name : VASANTHAN.N
### Reg no.: 212224240180
# Aim: Write a python program to check the number is prime or not and inspect for failures. 

# Algorithm
1. Start the program.
2. Get the number to be checked from the user.
3. If the number is less than or equal to 1, return "Not Prime".
4. If the number is 2, return "Prime".
5. Start the iteration from 3, For each iteration:
 - If the number is divisible by the current iteration value, return "Not Prime".
6. If the number is not divisible by any value from 2 to the square root, return "Prime".
7. Stop the program. 

## Program
```python
num = input("Enter a number: ")  
flag = 0  
if num.isnumeric():  
    z = int(num)  
    if z == 2:  
        flag = 1  
    elif z > 2:  
        for i in range(2, z // 2 + 1):  # Loop should include z//2
            if z % i == 0:  
                flag = 0  
                break  
        else:  
            flag = 1  
    if flag == 1:  
        print("Prime Number")  
    else:  
        print("Not a Prime Number")  
else:  
    print("Enter a Positive Number")
```
## Output

<img width="376" height="139" alt="Screenshot 2025-08-25 103127" src="https://github.com/user-attachments/assets/9fe9ef47-78dd-4115-af19-b13b492a5c57" />

<img width="375" height="115" alt="Screenshot 2025-08-22 114541" src="https://github.com/user-attachments/assets/4f9a4e91-2dbc-4c3f-845e-b80aed83cced" />

<img width="366" height="116" alt="Screenshot 2025-08-25 103245" src="https://github.com/user-attachments/assets/aff5d76a-0393-4339-b2c7-730bf8c8e5d5" />

<img width="376" height="124" alt="Screenshot 2025-08-25 103208" src="https://github.com/user-attachments/assets/33a5a54f-28b3-43b0-88d9-1acaa3eae313" />

## Result
Thus, the python program to check the number is prime or not is implemented and the output is verified successfully.
