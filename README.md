import random


def NPC(Place):
    num = random.randrange(0, 100)
    if Place == "Village":
        if num < 20:
            print("Hey, I like shorts!")
        elif num < 30:
            print("DO A BARREL ROLL")
        elif num < 45:
            print("Sceince isn't about why, it's about why not!")
        elif num < 80:
            print("What is a man? A mierable little pile of secrets.")
        else:
            print("I used to be an adventurer like you. Then I took an arrow in the knee")
            
room = 1
if room == 1:
        print("You enter a strange little town you see... Someone? or maybe lot's of someones. it appears to look like a person but also like 4 other persons. It takes the shape of a child, a anthropomorphic Bunny, a scientist, a peot and a retired adventurer. Do you dare talk to it? (Y)es or (N)o")
        choice = input()
        if choice == 'Y':
            room = 2
        elif choice == 'N':
            room = 3
        else:
            print("That is not an option")
if room == 3:
        print("As you turn away from the amalgamation, it grabs your leg and pulls you closer. THE END.")
if room == 2:
        num = random.randrange(0, 100)
        if num < 99:
            NPC("Village")
            print("Do you wish to speak with them again? (Y)es or (N)o")
            choice = input()
            if choice == 'Y':
                room = 2
            elif choice == 'N':
                room = 3
            else:
                print("That is not an option")
        else:
            print("The Amalgamation grows tired of you and eats you. THE END.")
    
    
        
