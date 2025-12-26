import random

# generate random number between 1 and 100
n = random.randrange(1, 100)

# take user input
guess = int(input("Enter any number: "))

while n != guess:
    if guess < n:
        print("Too low")
        guess = int(input("Enter number again: "))
    elif guess > n:
        print("Too high!")
        guess = int(input("Enter number again: "))
    else:
        break

print("You guessed it right!!")
