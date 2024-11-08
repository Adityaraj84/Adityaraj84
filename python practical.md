import cmath  # For handling complex square roots

# 1.Function to find the roots
<pre> def find_roots(a, b, c):
    # Calculate the discriminant
    discriminant = cmath.sqrt(b**2 - 4*a*c)

    # Calculate the two roots using the quadratic formula
    root1 = (-b + discriminant) / (2 * a)
    root2 = (-b - discriminant) / (2 * a)

    return root1, root2

 Input coefficients
print("Enter the coefficients of the quadratic equation (ax^2 + bx + c = 0):")
a = float(input("Enter coefficient a: "))
b = float(input("Enter coefficient b: "))
c = float(input("Enter coefficient c: "))

Ensure a is not zero (it must be a quadratic equation)
if a == 0:
    print("The coefficient 'a' cannot be zero. Please enter a valid quadratic equation.")
else:
    # Call the function to find roots
    root1, root2 = find_roots(a, b, c)

    # Output the results
    
    print(f"The roots of the quadratic equation are: {root1} and {root2}")</pre>
# 2.write a programm to accept a number 'n'
# 1. check if 'n' is prime
<pre> def is_prime(n):
    if n <= 1:
        return false
    for i in range(2, int(**0.5) + 1):
        # check divisors from 2 to sqrt(n)
        if n % i == 0:    #if n is divisible by any other number than 1 and itself
            return false
        return true
    n = int(input("enter a number: "))
    if is_prime (n):
        print (f"(n) is a prime number.")
    else:
     print(f"(n) is not prime number.")
    </pre>
     
# 3.Write a Programm to create a pyramid of the character'*' and a reverse pyramid
<pre> def create_pyramid(rows):
    for i in range(1, rows + 1):
#printing space to center - align the stars
        print(' ' *(rows - 1) + '*' *(2 * i - 1))
n = int (input("enter the number of rows for the pyramid: "))
create_pyramid(n) </pre>

# 4. # Function to check the character type
<pre> def check_char_type(char):
    if char.isalpha():
        return "Letter"
    elif char.isdigit():
        return "Numeric digit"
    else:
        return "Special character"

# Input from the user
char = input("Enter a character: ")

# Ensure the user inputs only one character
if len(char) == 1:
    print(check_char_type(char))
else:
    print("Please enter only a single character.")
Enter a character: A
Letter
Enter a character: 7
Numeric digit
Enter a character: @
Special character
</pre>
# 5.# Function to check letter case
<pre> def check_letter_case(char):
    if char.isalpha():
        if char.isupper():
            return "Uppercase letter"
        elif char.islower():
            return "Lowercase letter"
    else:
        return "Not a letter"

#Input from the user
char = input("Enter a character: ")

#Ensure the user inputs only one character
if len(char) == 1:
    print(check_letter_case(char))
else:
    print("Please enter only a single character.")
</pre>
