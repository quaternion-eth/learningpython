#This game allows user to guess a number between range 1 to 1000 and responds if the number is higher or lower
#You can always quit the game by typing 0
#Part of my learning exercise
#Enjoy!
import random
number = random.randint(1,1000)
print(number) #TODO: Remove after testing / Have only put this line to check whether the program is working fine or not
guess = int(input("Enter your guess: "))

while (guess != number and guess != 0):
    if guess > number:
        print("Guess lower" )
        guess = int(input())
    elif guess < number:
        print("Guess higher:  ")
        guess = int(input())

if guess == 0:
    print("Game over, you quit")
else:
    print("Congrats you guessed correctly")
