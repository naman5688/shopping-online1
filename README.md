items = {"Book": 10, "Pen": 2, "Bag": 25}
cart = []

for item in items:
    choice = input(f"Do you want to buy {item} for ${items[item]}? (yes/no): ")
    if choice.lower() == "yes":
        cart.append(item)

total = sum(items[i] for i in cart)
print(f"\nYou bought: {', '.join(cart)}")
print(f"Total: ${total}")
