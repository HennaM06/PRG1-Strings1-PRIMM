# Task 3: Applied Implementation, Answers

Complete this alongside `BRIEF_T3.md`.

## Explain your approach

### 1. Why does `apply_discount_code` call `apply_standard_discount` instead of repeating its logic?

> It reuses an existing code rather than using the same discount pattern. This makes the programme simpler.

### 2. Trace `print_order_summary("Pen", 2.00, 2, "invalid")`

>It's invalid because it isn't 6 uppercase letters. £4 is below £50 threshold meaning no discount is going to be applied.

### 3. Why does the default value on `discount_code` matter?

>Ensures discount codes are optional

### 4. `isalpha()` vs `isalnum()` in `validate_discount_code`

>isalpha() checks that the code contains letters only whereas isalnum() allows both letters and numbers.
