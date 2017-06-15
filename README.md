# SSAssessment2017

import turtle
import random
import math


#Set up screen
wn = turtle.Screen()
wn.bgcolor("lightgreen")
#wn.bgpic("     ")
wn.tracer(3)

#Set up shapes

batman = wn.addshape("/Users/student/PycharmProjects/TaylorAssessment2017/Images/Batman.gif")


#Create Player Variable
player = turtle.Turtle()
player.shape("turtle")
player.color("blue")
player.shape("batman")
player.penup()
player.speed(0)


#Set speed variable
speed = 1


#Define functions

def turnleft():
    player.left(90)

def turnright():
    player.right(90)

def increasespeed():
    global speed
    speed += 1

def decreasespeed():
    global speed
    speed -= 1



#Set keyboard bindings
wn.listen()
wn.onkey(turnleft, "Left")
wn.onkey(turnright, "Right")
wn.onkey(increasespeed, "Up")
wn.onkey(decreasespeed, "Down")

#Loops

while True:
    player.forward(speed)



delay = input("Press Enter to finish.")
...............................................................................................................................

