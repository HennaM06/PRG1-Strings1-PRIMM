# Task 4: Test-Driven Completion, Answers

Complete this alongside `BRIEF_T4.md`.

## Explain your approach

### 1. Why does `remove_stock` call `get_quantity` instead of reading `inventory[item_name]` directly?

> Because it safely checks how much stock an item has. If an item hasn't been added, get_quantity will return 0. 

### 2. Trace `remove_stock` on an item never added to the inventory

> The function would return false and the inventory would not change.

### 3. Difference between `inventory["Sprocket"]` and `inventory.get("Sprocket", 0)`

> This expects sprocket to already exist as a key in the dictionary, if it doesn't exist Python would raise an error. This matters becayse if an item has never been added it should be treated as having 0 stock rather than an error.

### 4. Why does the `<=` threshold boundary matter in `low_stock_items`?

> Because it includes items exactly at the threshold.
