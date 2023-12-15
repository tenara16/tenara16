import os
import time
from pyfiglet import Fliglet
from colorama import Fore,init

init(autoreset=True)

def clear_screen():
    os.system('cls' if os.name =='nt' else 'clear')

def display_text_animation(text,delay=1.0,clear=True):
    fig=Figlet(font='slant')
    if clear:
        clear_screen()
    for line in text.splitlines():
        print(Fore.RED + fig.renderText(line))
        time.sleep(delay)

def ask_question(question):
    print(Fore.GREEN +question)
    response=input(fore.YELLOW + "Yes or No?: ").lower()
    return response

def main():
    display_text_animation("I",delay=0.5)
    display_text_animation("I Love",delay=0.5)
    display_text_animation("I Love You",delay=0.5)

    #Display static text like animation I Love You

    response=ask_question("You Love Me?")

    if response=='yes':
        display_text_animation("I Love",delay=0.5)
        display_text_animation("I Love You",delay=0.5)

        #Display static text like animation I Love You
        print(Fore.RED +"Hehe<3")

    elif response=='no':
        display_text_animation("H",delay=0.5)
        display_text_animation("Hh",delay=0.5)
        display_text_animation("Hhh",delay=0.5)
        display_text_animation("Hhhh",delay=0.5)
        display_text_animation("Hhhhh",delay=0.5)
        display_text_animation("Hhhhhh",delay=0.5)
        clear_screen()
        display_text_animation("Hhhhhhhhh:(",delay=0.5)

if __name__=="__main__":
    main()




  
