# 24game
It's a cheat sheet to make a 24 game
print("Welcome to the Game Cheat Sheet!")
numbers = input("Please enter two numbers (Ex:1,2):")
listofnumbers = numbers.split(",")
print(listofnumbers)
box = []
for i in listofnumbers:
   box.append(int(i))
print(box)

if box[0]+box[1] == 24:
    print(str(box[0])+"+"+str(box[1]))
if abs(box[0]-box[1]) == 24:
    if box[0] >= box[1]:
        print(str(box[0])+"-"+str(box[1]))
    elif box[0] <= box[1]:
        print(str(box[1])+"-"+str(box[0]))
if box[0]*box[1] == 24:
    print(str(box[0])+"*"+str(box[1]))
if box[0] >= box[1]:
    print(box[0],box[1])
    if box[0]/box[1] == 24:
        print(str(box[0])+"/"+str(box[1]))
if box[1] >= box[0]:
    if box[1]/box[0] == 24:
        print(str(box[1])+"/"+str(box[0]))
