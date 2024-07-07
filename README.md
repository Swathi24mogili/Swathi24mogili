

import random as rd
x=[["•"],["• •"],["• • •"]]
y=[["• •"],[" • "]]
z=["• •"]

def user_input():
    a=rd.randint(1,6)
    print("Roll The Dice .")
    x=input("Enter x to Roll the Dice . ?\n")
    if x.lower() == "x":
        #print(a)
        if a == 1:
            print(f"Your Roll is {a}")
            roll_1()
            i=input("Want to Roll Again? Y/N\n")
            if i.lower() == "y":
                user_input()
            elif i.lower()=="n":
                print("Thanks :)")
                pass
            else:
                print("Wrong - Input..\nTRY AGAIN")
                user_input()


        elif a == 2:
            print(f"Your Roll is {a}")
            roll_2()
            i=input("Want to Roll Again? Y/N\n")
            if i.lower() == "y":
                user_input()
            elif i.lower()=="n":
                print("Thanks :)")
                pass
            else:
                print("Wrong - Input..\nTRY AGAIN")
                user_input()


        elif a == 3:
            print(f"Your Roll is {a}")
            roll_3()
            i=input("Want to Roll Again? Y/N\n")
            if i.lower() == "y":
                user_input()
            elif i.lower()=="n":
                print("Thanks :)")
                pass
            else:
                print("Wrong - Input..\nTRY AGAIN")
                user_input()

        elif a == 4:
            print(f"Your Roll is {a}")
            roll_4()
            i=input("Want to Roll Again? Y/N\n")
            if i.lower() == "y":
                user_input()
            elif i.lower()=="n":
                print("Thanks :)")
                pass
            else:
                print("Wrong - Input..\nTRY AGAIN")
                user_input()

        elif a == 5:
            print(f"Your Roll is {a}")
            roll_5()
            i=input("Want to Roll Again? Y/N\n")
            if i.lower() == "y":
                user_input()
            elif i.lower()=="n":
                print("Thanks :)")
                pass
            else:
                print("Wrong - Input..\nTRY AGAIN")
                user_input()

        elif a == 6:
            print(f"Your Roll is {a}")
            roll_6()
            i=input("Want to Roll Again? Y/N\n")
            if i.lower() == "y":
                user_input()
            elif i.lower()=="n":
                print("Thanks :)")
                pass
            else:
                print("Wrong - Input..\nTRY AGAIN")
                user_input()

    else:
        print("Wrong - Input..\nTRY AGAIN")
        user_input()

def roll_3():
    for i in x:
        if x.index(i) == 2:
            #Three
            print(f"{i}")

def roll_1():
    for i in x:
        if x.index(i) == 0:
            #One
            print(f"{i}")
        break

def roll_2():
    for i in x:
        if x.index(i) == 1:
            #Two
            print(f"{i}")

def roll_4():
    for i in y:
        if y.index(i) == 1:
            break
        #Four
        print(f"{i}\n{i}")


def roll_5():
    #Five
    print(f"{z}")

    for i in y:
        if y.index(i) == 1:
            print(f"{i}")
            print(z)

def roll_6():
    for i in x:
        if x.index(i) == 2:
            #Six
            print(f"{i}")
            print(i)

user_input()
     
Roll The Dice .
Enter x to Roll the Dice . ?
22
Wrong - Input..
TRY AGAIN
Roll The Dice .
Enter x to Roll the Dice . ?
Y
Wrong - Input..
TRY AGAIN
Roll The Dice .
Enter x to Roll the Dice . ?
X
Your Roll is 4
['• •']
['• •']
Want to Roll Again? Y/N
yy
Wrong - Input..
TRY AGAIN
Roll The Dice .
Enter x to Roll the Dice . ?
x
Your Roll is 3
['• • •']
Want to Roll Again? Y/N
y
Roll The Dice .
Enter x to Roll the Dice . ?
X
Your Roll is 3
['• • •']
Want to Roll Again? Y/N
y
Roll The Dice .
Enter x to Roll the Dice . ?
X
Your Roll is 1
['•']
Want to Roll Again? Y/N
N
Thanks :)
