# Section D -

## 1. (a) Guess the Output

Given:
```python
# Last 3 digits of ID = 257
x = 257 % 9

if x % 2 == 0:
    if x % 3 == 0:
        output = "Divisible by both 2 and 3"
    else:
        output = "Divisible by 2 only"
else:
    output = "Not divisible by 2"
print(output)
```

### Calculation:
- `x = 257 % 9 = 5`
- Since `5 % 2 != 0`, it goes to the `else` statement.

**Output:**
```
Not divisible by 2
```

---

## 1. (b) Guess the Output

```python
my_list = [3, 6, 9, 12, 15]
output = my_list.pop() + my_list[-1]
print(output)
```

### Execution:
1. `my_list.pop()` removes and returns `15`.
2. `my_list[-1]` refers to `12`.
3. `output = 15 + 12 = 27`.

**Output:**
```
27
```

---

## 2. Calculate Age & Senior Citizen Discount Eligibility

```python
birth_year = int(input("Enter your birth year: "))
current_year = 2025  # Assuming current year is 2025
age = current_year - birth_year

if age >= 60:
    print("Eligible for senior citizen discount.")
else:
    years_left = 60 - age
    print(f"Not eligible. You need {years_left} more years.")
```

### Example Outputs:
- **Input:** `1960` → **Output:** `Eligible for senior citizen discount.`
- **Input:** `1990` → **Output:** `Not eligible. You need 25 more years.`

---

## 3. Find the Longest Word(s) in a List

```python
words = ["apple", "banana", "grapefruit", "kiwi", "orange"]

if not words:
    print("The list is empty.")
else:
    max_length = max(len(word) for word in words)
    longest_words = [word for word in words if len(word) == max_length]
    print("Longest word(s):", longest_words)
```

### Execution:
- `"grapefruit"` is the longest word (length `10`).

**Output:**
```
Longest word(s): ['grapefruit']
```

