# Coffee Machine Project

## Overview

This project simulates a coffee machine that can serve three types of coffee: espresso, latte, and cappuccino. It handles resource management, monetary transactions, and provides reports on available resources and profits.

## Features

- **Menu Options:** Users can choose from three drinks: `espresso`, `latte`, and `cappuccino`.
- **Resource Management:** The machine checks if there are sufficient resources (water, milk, coffee) to make the selected drink.
- **Monetary Transactions:** The machine accepts coins (quarters, dimes, nickels, and pennies), calculates the total amount inserted, and checks if the payment is sufficient. If the payment is more than the drink cost, it returns the change.
- **Reports:** Users can request a report to see the remaining resources (water, milk, coffee) and the total profit.

## Code Breakdown

- **MENU Dictionary:** Contains the ingredients and cost for each drink option.
- **Resources Dictionary:** Tracks the current amount of available resources.
- **Functions:**
  - `is_resource_sufficient(order_ingredients)`: Checks if there are enough resources to make the selected drink.
  - `process_coins()`: Prompts the user to insert coins and calculates the total amount.
  - `is_transaction_successful(money_received, drink_cost)`: Validates if the user has inserted enough money and updates the profit.
  - `make_coffee(drink_name, order_ingredients)`: Deducts the required resources to make the drink and provides the coffee.
  
## How to Run

1. **Clone the repository** to your local machine.
2. **Run the script** using Python. You'll be prompted to select a drink.
3. **Follow the prompts** to insert coins and receive your drink.
4. **Check the report** by typing `report` to see the remaining resources and profit.
5. **Turn off the machine** by typing `off`.

## Example

```bash
What would you like? (espresso/latte/cappuccino): latte
Please insert coins.
how many quarters?: 10
how many dimes?: 0
how many nickles?: 0
how many pennies?: 0
Here is $0.0 in change.
Here is your latte ☕️. Enjoy!
