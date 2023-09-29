# Guess-Number_Python

```python
from random import randint

secret_number = randint(1, 100)
name = input('Your nane: ')
value = 0

print(f"Hello {name}, I've thought a number between 1 and 100 \n You have 8 attempts to guess it.")

for attempt in range(8):
    value = int(input("What is the number: "))

    if value < secret_number:
        print("My number is higher")

    elif value > secret_number:
        print("My number is lower")

    elif value == secret_number:
        print(f"Congratulations {name}! You guess it in {attempt + 1} attempts")
        break

if value != secret_number:
    print(f"I'm sorry, you have used all your attempts. The secret number was {secret_number}")

```
