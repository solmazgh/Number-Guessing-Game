# Number-Guessing-Game

import random
flag=True
count=0
y=random.randint(1, 9)
while flag and count<4:
 x=int(input("Enter a number you guess:(1-9) ")) count=count+1 if x==y: print("Congrats, your guess is correct") exit(0) elif x>y: print("your guess is too high") elif y>x: print("your guess is too low") elif x not in range(0,10): print("wrong input") if count==4: print("you exceeded your tree times chance") exit(0) quit=input("would you like to play again:(yes/no)")
 if quit.upper()=="No": flag=False
