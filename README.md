# Snake-Water-Gun
import random
computer = random.choice([-1,0,1])
youstr = input("Enter your choice : ")
youDic = {"s": 1,"w":-1 ,"g":0 }
reverseDic = {1 : "snack",-1 : "water" , 0 : "gun"}
you = youDic[youstr]
print(f"you chose: {reverseDic[you]}\ncomputer chose: {reverseDic[computer]} ")
if(computer == you):
    print("Its Draw!")
else:
    if(computer == -1 and you == 1):
        print("You Win!")
    elif(computer == -1 and you == 0):
        print("You Lose!")
    if(computer == 1 and you == 0):
        print("You Win!")
    elif(computer == 1 and you == -1):
        print("You Lose!")
    if(computer == 0 and you == -1):
        print("You Win!")
    elif(computer == 0 and you == 1):
        print("You Lose!")
