# Rock_Paper_scissor_in_python
import random
rock = '''
    _______
---'   ____)
      (_____)
      (_____)
      (____)
---.__(___)
'''

paper = '''
    _______
---'   ____)____
          ______)
          _______)
         _______)
---.__________)
'''

scissors = '''
    _______
---'   ____)____
          ______)
       __________)
      (____)
---.__(___)
'''
list_rps=[rock,paper,scissors]
length=len(list_rps)
# print(list_rps[2])
#Write your code below this line 👇
my=int(input("What do you choose? Type 0 for Rock, 1 for Paper or 2 for Scissors.\n"))
if (my==0) or (my==1) or (my==2):
  if (my==0) :
    print(rock)
    print("Computer Choose")
    n=random.choice(list_rps)
    print(n)
    if (rock)==(n):
      print("draw")
    elif (paper)==(n):
      print("Computer Win")
    elif(scissors)==(n):
      print("You Win")
  
  if (my==1) :
    print(paper)
    print("Computer Choose")
    n=random.choice(list_rps)
    print(n)
    if (rock)==(n):
      print("You Win")
    elif (paper)==(n):
      print("Draw")
    elif(scissors)==(n):
      print("Computer Win")

  if (my==2) :
    print(scissors)
    print("Computer Choose")
    n=random.choice(list_rps)
    print(n)
    if (rock)==(n):
      print("You lose")
    elif (paper)==(n):
      print("You Win")
    elif(scissors)==(n):
      print("Draw")
else:
  print('invalid entry, Try Again')
