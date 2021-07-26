# codes4guessinggame
import random
secret_number=random.randint(1,10)
guess=0
c=0
while int(guess)!=secret_number:
    guess=input("please take a guess: ")
    c=c+1
    if int(guess)<secret_number:
        print("your guess is too low")
        continue
    if int(guess)>secret_number:
        print("your guess is too high")
        continue
    else:
        break
    
print("you guessed it correctly in {} times".format(c))

