# Online-Shopping-System

## Overview
This project implements a simple Online Shopping System in Python. It includes classes for various product types, order management, and delivery charges. The example usage demonstrates the creation of electronic items, grocery items, and a laptop, which are added to an order with specific quantities. The order details, including delivery method and address, are displayed along with the total bill.

## Project Structure
- `product.py`: Contains the base `Product` class and its subclasses (`ElectronicItem`, `GroceryItem`, `Laptop`).
- `order.py`: Defines the `Order` class for managing customer orders and delivery charges.

## Usage
1. Create instances of products (e.g., TV, Milk, Laptop).
2. Initialize an order with a delivery method and address.
3. Add items to the order using the `add_item` method.
4. Update delivery charges using the `update_delivery_charges` method.
5. Display order details using the `display_order_details` method.

## Example
```python
# Example Usage
tv = ElectronicItem("TV", 45000, 40000, 4.7, 24)
milk = GroceryItem("Milk", 70, 60, 4.0, "Jan 2023")
lenovo_lap = Laptop("Lenovo 123", 45000, 30000, 4.5, 24, "16 GB", "1 TB SSD")

my_order = Order("Normal", "Hyderabad")
my_order.add_item(tv, 1)
my_order.add_item(milk, 3)
my_order.add_item(lenovo_lap, 1)
my_order.update_delivery_charges("Normal", 100)
my_order.display_order_details()

