[README(7).md](https://github.com/user-attachments/files/32071995/README.7.md)
```python
def calculate_final_price(price, discount_rate):
    discount = price * discount_rate
    final_price = price - discount
    return final_price

# Test the function
result = calculate_final_price(1200, 0.15)

print("Final Price:", result)
```

**Output:**
```text
Final Price: 1020.0
```

```python
def get_delivery_charge(amount, city='Ahmedabad'):
    if city == 'Ahmedabad':
        return 30
    else:
        return 50


# Without city argument
print("Ahmedabad:", get_delivery_charge(500))

# With city argument
print("Mumbai:", get_delivery_charge(500, 'Mumbai'))
```

**Output:**
```text
Ahmedabad: 30
Mumbai: 50
```

```python
def format_coupon_message(username, discount=10):
    return f"Hi {username}, you get {discount}% off!"


# Custom discount
print(format_coupon_message("Shiv", 20))

# Default discount
print(format_coupon_message("Dixit"))
```

**Output:**
```text
Hi Shiv, you get 20% off!
Hi Dixit, you get 10% off!
```

```python
def apply_discount(price, rate=0.10):
    discount = price * rate
    final_price = price - discount
    return final_price


# Call with only price
result = apply_discount(1000)

print("Final Price:", result)
```

**Output:**
```text
Final Price: 900.0
```

```python
def calculate_cashback(amount, cashback_rate=0.05):
    cashback = amount * cashback_rate
    return cashback


# Zomato order - default 5% cashback
zomato_cashback = calculate_cashback(500)

# Flipkart order - custom 7% cashback
flipkart_cashback = calculate_cashback(2000, 0.07)

print("Zomato Cashback:", zomato_cashback)
print("Flipkart Cashback:", flipkart_cashback)
```

**Output:**
```text
Zomato Cashback: 25.0
Flipkart Cashback: 140.0
```
