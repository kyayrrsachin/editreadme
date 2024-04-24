# editreadme
--------------------Q1

a=5
b=6

addition= a+b
substraction= a-b
multiplication= a*b

print("arithmetic operators:")
print("a=5 b=6")
print("addition:",addition)
print("substraction:",substraction)
print("multiplication:",multiplication)

x=True
y=False

logical_and= x and y
logical_or= x or y
logical_not= not x

print("\nlogical operators:")
print("x=true y=false")
print("logical AND:",logical_and)
print("logical OR:",logical_or)
print("logical NOT:",logical_not)

m=10
n=5
bitwise_and= m&n
bitwise_or= m|n
bitwise_xor= m^n

print("\nbitwise operator:")
print("m=10 n=5")
print("bitwise AND:",bitwise_and)
print("bitwise OR:",bitwise_or)
print("bitwise XOR:",bitwise_xor)

p=6
q=9
greater_than= p>q
less_than_or_equal_to= p<=q
equal_to= p==q

print("\nrealtional operator")
print("p=6 q=9")
print("greater than:",greater_than)
print("less than or equal to:",less_than_or_equal_to)
print("equal to:",equal_to)

---------------------------------Q2 

------(a)
row = int(input("enter the number of rows: "))

for i in range (row):
    print(" "*(row-i)+" *"*(i+1))

for j in range(row-1):
    print(" "*(j+2)+" *"*(row-1-j))

------(b)
rows=int(input("enter the number of rows: "))
for i in range(1,rows+1):
    for j in range(rows-i):
        print(" ",end="")
    for k in range(i,2*i):
        print(k,end="")
    for l in range(2*i-2,i-1,-1):
        print(l,end="")
    print()

------------------------Q3
import math

print("Pi:", math.pi) 

angle = math.radians(45)
print("Sine of 45 degrees:", math.sin(angle))
print("Cosine of 45 degrees:", math.cos(angle))


print("Natural logarithm of 10:", math.log(10))
print("Exponential of 2:", math.exp(2))

print("2 raised to the power of 3:", math.pow(2, 3)) 
print("Square root of 16:", math.sqrt(16))

print("Ceiling of 4.5:", math.ceil(4.5)) 
print("Floor of 4.5:", math.floor(4.5))

Q4
import math

# Input lengths of the sides from the user
side1 = float(input("Enter the length of side1: "))
side2 = float(input("Enter the length of side2: "))
side3 = float(input("Enter the length of side3: "))

# Check triangle inequality theorem
if side1 + side2 > side3 and side2 + side3 > side1 and side1 + side3 > side2:

    s = (side1 + side2 + side3) / 2

    # Calculate area using Heron's formula
    area = math.sqrt(s * (s - side1) * (s - side2) * (s - side3))
    print("Area of the triangle:", area)
else:
    print("The sum of the lengths of any two sides is not greater than the third side.")

---------------------Q5

num = int(input("Enter a number to compute its factorial: "))
if num < 0:
    print("Factorial is not defined for negative numbers.")
else:
    result = 1
    for i in range(1, num + 1):
        result *= i
    print("Factorial of", num, "is:", result)


