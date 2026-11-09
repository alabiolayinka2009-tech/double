def is_triple_multiple_of_double(num1, num2):
    """
    Determines whether the first number tripled (num1 * 3) 
    is a multiple of the second number doubled (num2 * 2) 
    using the remainder operator (%).
    """
    tripled = num1 * 3
    doubled = num2 * 2
    
    # A number is a multiple if the remainder is 0
    if doubled != 0 and tripled % doubled == 0:
        return True
    return False

def main():
    # Read two integers from the user
    num1 = int(input("Enter first integer: "))
    num2 = int(input("Enter second integer: "))

    # Determine and print the result[cite: 3]
    result = is_triple_multiple_of_double(num1, num2)
    
    if result:
        print(f"Yes, {num1} tripled ({num1 * 3}) is a multiple of {num2} doubled ({num2 * 2})[cite: 3].")
    else:
        print(f"No, {num1} tripled ({num1 * 3}) is not a multiple of {num2} doubled ({num2 * 2})[cite: 3].")

if __name__ == "__main__":
    main()
