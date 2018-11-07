# Text-Adventure-

import time
import random

print ("You have arrived upstairs. You see a room in front of you and to your right.")
def ask(question):
    answer = input(question + "[f/r]")
    return answer in ['r', 'R', 'Right', "right", 'RIGHT']
    #front room
ct = True
while ct:
  room = str(input("Do you go to the room in front of you or to your right? [f/r]: "))
  if room == "f":
      ct= False
      print ("You have chosen the door in front of you. You look around the dark room and see a door on the opposite side of the room of where you stand.")
      door = str(input("Do you go to the door and look through it? [y/n]: "))
      if door.lower() in ['y', 'yes']:
          print ("You have gone through the door and are in a newroom now.")
          print ("You realize that the new room you are in is a living room and that nothing sticks out.")
          print ("You figure out that upstairs has nothing to help you get out of this strange house. And that you have to go downstairs again and look harder.")
      elif door.lower() in ['n','no']:
          print ("Curiosity is going to get to you. I know you want to go through it. But your loss.")
      else:
        print ("I don't know what that is.")
    #bathroom
  if room == "r":
      print ("You have chosen the door to the right of you. You notice that it is a bathroom. ")
      print ("You look around and see that there is nothing there. Just a boring empty dark room. ")
