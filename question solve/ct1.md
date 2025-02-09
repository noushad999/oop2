##Section_D
1. (a) Guess the Output:
Given:

Last 3 digits of ID = 257
Compute x = 257 % 9
Let's calculate:

257
÷
9
=
28
 remainder 
5
257÷9=28 remainder 5
So, x = 5

Now checking conditions:

5 % 2 == 0 (False) → Goes to else statement
Output: "Not divisible by 2"
Final Output:

csharp
Copy
Edit
Not divisible by 2
1. (b) Guess the Output:
python
Copy
Edit
my_list = [3, 6, 9, 12, 15]
output = my_list.pop() + my_list[-1]
print(output)
Step-by-step execution:

my_list.pop() removes and returns the last element → 15
my_list[-1] now refers to 12 (new last element after pop)
output = 15 + 12 = 27
print(output)
Final Output:

Copy
Edit
27
2. Calculate Age & Senior Citizen Discount Eligibility:
python
Copy
Edit
birth_year = int(input("Enter your birth year: "))
current_year = 2025  # Assuming current year is 2025
age = current_year - birth_year

if age >= 60:
    print("Eligible for senior citizen discount.")
else:
    years_left = 60 - age
    print(f"Not eligible. You need {years_left} more years.")
Example Outputs:

Input: 1960 → "Eligible for senior citizen discount."
Input: 1990 → "Not eligible. You need 25 more years."
3. Find the Longest Word(s) in a List:
python
Copy
Edit
words = ["apple", "banana", "grapefruit", "kiwi", "orange"]

if not words:
    print("The list is empty.")
else:
    max_length = max(len(word) for word in words)
    longest_words = [word for word in words if len(word) == max_length]
    print("Longest word(s):", longest_words)
Execution:

"grapefruit" is the longest word (length 10).
Output:
scss
Copy
Edit
Longest word(s): ['grapefruit']
