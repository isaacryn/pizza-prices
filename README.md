# pizza-prices
modifying prices in python
# List of toppings
toppings = ["pepperoni", "pineapple", "cheese", "sausage", "olives", "anchovies", "mushrooms"]

# List of prices
prices = [2, 6, 1, 3, 2, 7, 2]

# Count occurrences of $2 slices
num_two_dollar_slices = prices.count(2)
print(num_two_dollar_slices)  # Outputs the number of $2 slices

# Find the number of different kinds of pizza
num_pizzas = len(toppings)
print(f"We sell {num_pizzas} different kinds of pizza!")  # Prints the number of pizzas

# Create a 2D list of pizza prices and toppings
pizza_and_prices = [
    [2, "pepperoni"],
    [6, "pineapple"],
    [1, "cheese"],
    [3, "sausage"],
    [2, "olives"],
    [7, "anchovies"],
    [2, "mushrooms"]
]

# Print the pizza_and_prices list
print(pizza_and_prices)

# Sort the pizzas by price (ascending order)
pizza_and_prices.sort()
print("Sorted pizzas by price:", pizza_and_prices)

# Store the cheapest pizza
cheapest_pizza = pizza_and_prices[0]
print("Cheapest pizza:", cheapest_pizza)

# Store the most expensive pizza
priciest_pizza = pizza_and_prices[-1]
print("Priciest pizza:", priciest_pizza)

# Remove the most expensive pizza (anchovies)
pizza_and_prices.pop()  # Removes the last item which is the priciest pizza (anchovies)
print("After removing the priciest pizza:", pizza_and_prices)

# Add the new "peppers" topping with a price of $2.5, and insert it in the correct position
pizza_and_prices.append([2.5, "peppers"])
pizza_and_prices.sort()  # Resort the list to maintain order by price
print("After adding 'peppers':", pizza_and_prices)

# Slice the list to get the three cheapest pizzas
three_cheapest = pizza_and_prices[:3]
print("Three cheapest pizzas:", three_cheapest)
