import random

def gameWin(comp, you):
    if comp == you :
       return None
    elif you == 's':
        if you=='w':
          return False

        elif you == 'g':
            return True   
print("comp Turn: Snake(s) Water(w) or Gun(g)?")
randNo = random.randint(1,2)
print(randNo)
if randNo == 1:
 comp = 's' 
elif randNo == 2:
    comp = 'w'
elif randNo == 1:
    comp = 'g'

 
you = input("you Turn: Snake(s) Water(w) or Gun(g)?") 
a = gameWin(comp, you)
if a == None:
    print("game is a tie")
elif a:
    print("you win")
else:
    print("you lose")
    
