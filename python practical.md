import cmath  # For handling complex square roots

# Function to find the roots
def find_roots(a, b, c):
    # Calculate the discriminant
    discriminant = cmath.sqrt(b**2 - 4*a*c)

    # Calculate the two roots using the quadratic formula
    root1 = (-b + discriminant) / (2 * a)
    root2 = (-b - discriminant) / (2 * a)

    return root1, root2

# Input coefficients
print("Enter the coefficients of the quadratic equation (ax^2 + bx + c = 0):")
a = float(input("Enter coefficient a: "))
b = float(input("Enter coefficient b: "))
c = float(input("Enter coefficient c: "))

# Ensure a is not zero (it must be a quadratic equation)
if a == 0:
    print("The coefficient 'a' cannot be zero. Please enter a valid quadratic equation.")
else:
    # Call the function to find roots
    root1, root2 = find_roots(a, b, c)

    # Output the results
    print(f"The roots of the quadratic equation are: {root1} and {root2}")
# write a programm to accept a number 'n'
# 1. check if 'n' is prime
def is_prime(n):
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
