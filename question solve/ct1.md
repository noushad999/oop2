# Section C 
# Set 1

## 1. List Slicing and Operations

Given:
```python
my_list = [5, 10, 15, 20, 25, 30, 35, 40, 45]
```

### (a) Obtain `[10, 25, 40]` using slicing:
```python
output1 = my_list[1::3]
print(output1)
```
**Output:**
```
[10, 25, 40]
```

### (b) Obtain `[45, 40, 35]` using slicing:
```python
output2 = my_list[-1:-4:-1]
print(output2)
```
**Output:**
```
[45, 40, 35]
```

### (c) What is the output of:
```python
print(my_list.pop() == my_list[-1])
```
**Execution:**
- `my_list.pop()` removes and returns `45`.
- `my_list[-1]` now refers to `40`.
- Since `45 != 40`, the output is:
```
False
```

### (d) Sum of all elements in `my_list`:
```python
sum_list = sum(my_list)
print(sum_list)
```

### (e) Obtain substring `"World"` from `my_string`:
```python
my_string = "Hello, World!"
substring = my_string[7:12]
print(substring)
```
**Output:**
```
World
```

---

## 2. Voting Eligibility Check

```python
age = int(input("Enter your age: "))
if age >= 18:
    print("Eligible to vote.")
else:
    years_left = 18 - age
    print(f"Not eligible. You need {years_left} more years.")
```

### Example Outputs:
- **Input:** `20` → **Output:** `Eligible to vote.`
- **Input:** `16` → **Output:** `Not eligible. You need 2 more years.`

---

## 3. Counting Even and Odd Numbers in a List

```python
numbers = [12, 7, 5, 8, 14, 9, 22, 13, 18, 21]

count_even = sum(1 for num in numbers if num % 2 == 0)
count_odd = len(numbers) - count_even

print(f"Even count: {count_even}, Odd count: {count_odd}")

if count_even > count_odd:
    print("More evens")
elif count_odd >= count_even:
    print("More odds")
```

### Example Execution:
**Output:**
```
Even count: 5, Odd count: 5
More odds
```

# Set 2

## 1. List Slicing and Operations

Given:
```python
my_list = [1, 3, 5, 7, 9, 11, 13, 15, 17]
```

### (a) Obtain `[3, 9, 15]` using slicing:
```python
output1 = my_list[1::3]
print(output1)
```
**Output:**
```
[3, 9, 15]
```

### (b) Obtain `[17, 15, 13]` using slicing:
```python
output2 = my_list[-1:-4:-1]
print(output2)
```
**Output:**
```
[17, 15, 13]
```

### (c) What is the output of:
```python
print(my_list[-1] == my_list.pop())
```
**Execution:**
- `my_list.pop()` removes and returns `17`.
- `my_list[-1]` now refers to `15` before the pop.
- Since `17 == 17`, the output is:
```
True
```

### (d) Sum of all elements in `my_list`:
```python
sum_list = sum(my_list)
print(sum_list)
```

### (e) Obtain substring `"Hello"` from `my_string`:
```python
my_string = "Hello, World!"
substring = my_string[:5]
print(substring)
```
**Output:**
```
Hello
```

---

## 2. Voting Eligibility Check

```python
age = int(input("Enter your age: "))
if age >= 18:
    print("Eligible to vote.")
else:
    years_left = 18 - age
    print(f"Not eligible. You need {years_left} more years.")
```

### Example Outputs:
- **Input:** `20` → **Output:** `Eligible to vote.`
- **Input:** `16` → **Output:** `Not eligible. You need 2 more years.`

---

## 3. Counting Even and Odd Numbers in a List

```python
numbers = [12, 7, 5, 8, 14, 9, 22, 13, 18, 21]

count_even = sum(1 for num in numbers if num % 2 == 0)
count_odd = len(numbers) - count_even

print(f"Even count: {count_even}, Odd count: {count_odd}")

if count_even > count_odd:
    print("More evens")
elif count_odd >= count_even:
    print("More odds")
```

### Set 2
**Output:**
```
Even count: 5, Odd count: 5
More odds
```



# Section D -

# Set 1


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

# Set 2

## 1. (a) Guess the Output

Given:
```python
# Last 3 digits of ID = 257
x = 257 % 5

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
- `x = 257 % 5 = 2`
- Since `2 % 2 == 0`, it enters the first `if`.
- Since `2 % 3 != 0`, it enters the `else`.

**Output:**
```
Divisible by 2 only
```

---

## 1. (b) Guess the Output

```python
my_list = [3, 6, 9, 15, 15]
output = my_list.pop() + my_list[-1]
print(output)
```

### Execution:
1. `my_list.pop()` removes and returns `15`.
2. `my_list[-1]` refers to `15`.
3. `output = 15 + 15 = 30`.

**Output:**
```
30
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

