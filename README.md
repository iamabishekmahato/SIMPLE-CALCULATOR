# SIMPLE-CALCULATOR
calculate odd or even, simple interest and use for two number calculate 

print("================================")
print("       CGA ABISHEK CALCULATOR")
print("================================")

print("\nChoose what you want to calculate:")
print("1. Odd or Even")
print("2. Simple Interest")
print("3. Simple Calculator")

choice = int(input("\nEnter your choice (1-3): "))

# 1. Odd or Even
if choice == 1:
    num = int(input("Enter a number: "))

    if num % 2 == 0:
        print(num, "is Even")
    else:
        print(num, "is Odd")

# 2. Simple Interest
elif choice == 2:
    p = float(input("Enter Principal: "))
    r = float(input("Enter Rate (%): "))
    t = float(input("Enter Time (years): "))

    si = (p * r * t) / 100

    print("Simple Interest =", si)
    print("Total Amount =", p + si)

# 3. Simple Calculator
elif choice == 3:
    a = float(input("Enter first number: "))
    op = input("Enter operator (+, -, *, /): ")
    b = float(input("Enter second number: "))

    if op == "+":
        print("Answer =", a + b)

    elif op == "-":
        print("Answer =", a - b)

    elif op == "*":
        print("Answer =", a * b)

    elif op == "/":
        if b != 0:
            print("Answer =", a / b)
        else:
            print("Cannot divide by zero!")

    else:
        print("Invalid operator!")

else:
    print("Invalid choice!")

print("\n===== THANK YOU =====")
print("       BY CGA 😈")
