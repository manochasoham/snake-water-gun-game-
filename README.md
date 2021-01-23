# snake-water-gun-game-

print("welocome to the game")
#print("choose snake ,water ,gun")
import random
user_point=0
computer_point=0
attempts=1
while attempts<=10:
    
     
    lst=["snake","water","gun"]
    choice=random.choice(lst)
    num=input("choose snake water gun\n")
    if num==choice:
        print("tie")
        print(f"you choose{num}  and computer chosse {choice}")
    elif num=="snake" and choice=="water":
        print("you choose{num} and computer choose {choice}")
        print("you win snake drank water")
        user_point=user_point+1
    elif num=="snake" and choice=="gun":
        print(f"you choose{num} and computer chosse {choice}")
        print("you loose gun shootes snake")
        computer_point=computer_point+1
    elif num=="water" and choice=="snake":
        print(f"you choose{num} and computer chosse {choice}")
        print("you lose snake drank water")
        computer_point=computer_point+1
    elif num=="water" and choice=="gun":
        print(f"you choose{num} and computer chosse {choice}")
        print("you win gun sink into water")
        user_point=user_point+1
    elif num=="gun" and choice=="snake":
        print(f"you choose{num }  and computer chosse   {choice}")
        print("you win")
        user_point=user_point+1
    elif num=="gun" and choice=="water":
        print(f"you choose{num} and computer chosse {choice}")
        print("you lose")
        computer_point=computer_point+1
    else:
        print("invalid")
        
        
        if attempts>10:
            print("game over")
            
        
        if user_point>computer_point:
            print("user win")
        else:
            print("computer win")
            
            print(10-attempts,"no of guesses left")
    attempts=attempts+1
        
    print(f"your point is { user_point} and computer point is {computer_point
