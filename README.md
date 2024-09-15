def take_pizza_order():
    size = input("Enter pizza size (S, M, L): ").upper()
    pepperoni = input("Do you want pepperoni? (Y/N): ").upper()
    extra_cheese = input("Do you want extra cheese? (Y/N): ").upper()
    extra= input("Do you want anything else? (Y/N): ").upper()
    bill = 0
    if size == "S":
        bill = 100
    elif size == "M":
        bill = 200
    elif size == "L":
        bill = 300

    if pepperoni == "Y":
        bill += 100
    if extra_cheese == "Y":
        bill += 50
    if extra == "Y":
        what= input("What do you want: ")
        print("Sorry we dont have ",what)

    print("Your final bill is: ", bill)

take_pizza_order()
