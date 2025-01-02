# Python-Programming- A small Ordering Sweets

menu={
    'Roshogolla':10,
    'Pantua':7,
    'Kalakand':10,
    'Kheerkodom':10,
    'Rasmalai':15
    
}
print('Welcome to Lucky Sweet's 🥰')
print("Roshogolla: Rs10\nPantua: Rs7\nKalakand: Rs10\nKheerkodom: Rs10\nRasmalai: Rs15\n")
print("-------------------------------------------")
order_total = 0
item_1 = input("Enter the name of item you want to order:- ")
if item_1 in menu:
    order_total +=menu[item_1]
    print(f"Your item {item_1} has been added to your order")
else:
    print("Order item {item_1} is not avaialable yet")
another_order = input("Do you want to add another item? (Yes/No):")
if another_order == "Yes":
    item_2 =input("Enter the same of second item:=")
    if item_2 in menu:
        order_total +=menu[item_2]
        print(f"Item {item_2} has been added to order")
    else:
        print(f"Order item {item_2} is not avaialable!")

print(f"The total amount of items is {order_total}")   
print("Thankyou\nVisit Again")
