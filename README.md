# Python-W3

def calculate_discount(price, discount_percent):
    if discount_percent >= 20:
        discount_amount = (price / 100) * discount_percent
        final_price = price - discount_amount
        return final_price
    else:
        return price

def main():
    original_price = float(input("Enter the original price of the item: $"))
    discount_percent = float(input("Enter the discount percentage (%): "))

    final_price = calculate_discount(original_price, discount_percent)

    if final_price == original_price:
        print(f"No discount applied. The price remains: ${original_price:.2f}")
    else:
        print(f"The final price after applying the discount is: ${final_price:.2f}")

if __name__ == "__main__":
    main()
