# Smart Home Automation Program

light = False
fan = False
door = False

while True:
    print("\n===== SMART HOME AUTOMATION =====")
    print("1. Turn ON Light")
    print("2. Turn OFF Light")
    print("3. Turn ON Fan")
    print("4. Turn OFF Fan")
    print("5. Open Door")
    print("6. Close Door")
    print("7. View Device Status")
    print("8. Exit")

    choice = int(input("Enter your choice: "))

    if choice == 1:
        light = True
        print("Light is ON")

    elif choice == 2:
        light = False
        print("Light is OFF")

    elif choice == 3:
        fan = True
        print("Fan is ON")

    elif choice == 4:
        fan = False
        print("Fan is OFF")

    elif choice == 5:
        door = True
        print("Door is OPEN")

    elif choice == 6:
        door = False
        print("Door is CLOSED")

    elif choice == 7:
        print("\n----- Device Status -----")
        print("Light:", "ON" if light else "OFF")
        print("Fan:", "ON" if fan else "OFF")
        print("Door:", "OPEN" if door else "CLOSED")

    elif choice == 8:
        print("Thank you for using Smart Home Automation!")
        break

    else:
        print("Invalid choice! Please try again.")
