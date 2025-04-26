# Discount Calculator Program

## Overview

The **Discount Calculator Program** is a Python script that calculates the final price of an item based on a given discount percentage. The discount is only applied if it is 20% or greater; otherwise, the original price is returned.

## Features

- Prompts the user to input the original price of an item and a discount percentage.
- Applies a discount if the percentage is 20% or higher.
- Returns either the discounted price or the original price if the discount is less than 20%.
- User-friendly output for easy understanding of results.

## Requirements

- Python 3.x

## Codes

def calculate_discount(price, discount_percent):
    # Check if the discount percentage is 20% or greater
    if discount_percent >= 20:
        # Calculate the final price after applying the discount
        discount_amount = price * (discount_percent / 100)
        final_price = price - discount_amount
        return final_price
    else:
        # Return the original price if discount is less than 20%
        return price

# Prompt the user for input
original_price = float(input("Enter the original price of the item: "))
discount_percentage = float(input("Enter the discount percentage: "))

# Calculate the final price using the calculate_discount function
final_price = calculate_discount(original_price, discount_percentage)

# Print the result
if final_price == original_price:
    print(f"No discount applied. The original price is: ${final_price:.2f}")
else:
    print(f"The final price after applying the discount is: ${final_price:.2f}")
    

## Usage

1. Make sure you have Python 3 installed on your machine.
2. Download or copy the Python script.
3. Open a terminal or command prompt.
4. Navigate to the directory where the script is located.
5. Run the script using:

   ```bash
   python discount_calculator.py
