# Action-Menu---Abid-Hasan-Alnoor
#TBG Action Menu - Abid hasan Alnoor
#May 17, 2022
#This code will create an action menu for my game
import colorama
from colorama import Fore

actions= ['Attack','Defend', 'Heal','Run']
weapons= ['Sword' , 'Gauntlets', 'Sheild']


#Tis a little bit of text that will appear in the begining of my game 
print('Welcome to the world of .........')

#This funtion is the actual interactive menu 
def part():
    
    #This part will print the choices the player should make
    print(Fore.RED + 'Please Choose one of the following weapons')
    for equip in weapons:
        print('*' + equip)
    armory= input()
    
    print(Fore.RED + 'Complete one of the follwing actions')
    for choice in actions:
        print('*' + choice)
    act= input()
     
     #This part checks the user input for the attcking choice 
    if act== 'Attack' and armory== 'Sword' :
        print(Fore.YELLOW + 'You did 95 damage')
    elif act== 'Attack' and armory== 'Gauntlets' :
        print(Fore.YELLOW + 'You did 75 damage')
    elif act== 'Attack' and armory== 'Sheild' :
        print(Fore.YELLOW + 'You did 25 damage')
    
    #This part checks the user input for the defending choice 
    elif act== 'Defend' and armory== 'Sword' :
        print(Fore.YELLOW + 'You took 45 damage')
    elif act== 'Defend' and armory== 'Gauntlets' :
        print(Fore.YELLOW + 'You took 55 damage')
    elif act== 'Defend' and armory== 'Sheild' :
        print(Fore.YELLOW + 'You took 10 damage')
    
    #This part checks the user input for the run and heal choice 
    elif act== 'Heal' :
        print(Fore.YELLOW + 'You healed 40 damage')
    elif act== 'Run' :
        print(Fore.YELLOW + 'You somehow managed to escape')
    #This part check for mistakes in the input and reruns the funtions as needed  
    else :
        print (Fore.GREEN + 'Please check your spelling and try again')
        part()
    
    
    
        
    
    
        
        
part()
    
