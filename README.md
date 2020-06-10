# python
import random
winning_number=random.randint(1,100)
guess=1
game_over=False
number=int(input("enter the no. between 1 to 100"))
while not game_over:
  if winning_number == number:
    print(f"you win attempt{guess} time")
    game_over=True
  else:
    if number < winning_number:
      print("too low")
    else:
      print("too high")

    guess+=1
    number=int(input("guess again"))
      
