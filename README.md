# Python-Programming- A small Ordering Sweets

sweets_menu = {
    'Roshogolla': 190,
    'Gulab Jamun': 108,
    'Kalakand': 100,
    'Palakova': 120,
    'Rasmalai': 115
}

print("Welcome To Lucky Sweet House_!🥰")
print("\nRoshogolla: Rs.190\nGulab Jamun: Rs.108\nKalakand: Rs.100\nPalakova: Rs.120\nRasmalai: Rs.115\n")
print("------------------------------------------->>")

order_total = 0
item_1 = input("Enter the name of the item you want to order: ")

if item_1 in sweets_menu:
    order_total += sweets_menu[item_1]
    print(f"Your item '{item_1}' has been added to your order.")
else:
    print(f"Sorry, the item '{item_1}' is not available.")

another_order = input("Do you want to add another item? (Yes/No): ").strip().capitalize()

if another_order == "Yes":
    item_2 = input("Enter the name of the second item: ")
    if item_2 in sweets_menu:
        order_total += sweets_menu[item_2]
        print(f"Your item '{item_2}' has been added to your order.")
    else:
        print(f"Sorry, the item '{item_2}' is not available!")

print(f"The total amount of your order is Rs = {order_total}")
print("\nThank you! Visit again_🤗")
