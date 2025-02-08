start = int(input("Enter the starting number: "))
end = int(input("Enter the ending number: "))
update = int(input("Enter the update value (step): "))


print("\nChoose direction:")
print("1. Forward")
print("2. Reverse")
direction = int(input("Enter your choice (1 or 2): "))


print("\nChoose display orientation:")
print("H. Horizontal")
print("V. Vertical")
orientation = input("Enter your choice (H or V): ").upper()


if direction == 1: 
    if orientation == 'H':
      
        for num in range(start, end + 1, update):
            print(num, end=' ')
    elif orientation == 'V':
       
        for num in range(start, end + 1, update):
            print(num)
    else:
        print("Invalid orientation choice! Please enter 'H' or 'V'")

elif direction == 2: 
    if orientation == 'H':
       
        for num in range(start, end - 1, -update):
            print(num, end=' ')
    elif orientation == 'V':
      
        for num in range(start, end - 1, -update):
            print(num)
    else:
        print("Invalid orientation choice! Please enter 'H' or 'V'")

else:
    print("Invalid direction choice! Please enter 1 or 2")# Number-system
