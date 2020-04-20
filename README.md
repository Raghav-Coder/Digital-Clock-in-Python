# Digital-Clock-in-Python
import sys
from tkinter import *
import time

def times():
    current_time=time.strftime("%H:%M:%S")
    clock.config(text=current_time)
    clock.after(200, times)
    
root=Tk()
root.title("DIGITAL CLOCK BY Raghav")
root.geometry("700x320")
clock= Label(root, font=("arial", 50, "bold"), bg="white")
clock.grid(row=2, column=2, padx=25, pady=100)
times()

digi = Label(root, text="Digital Clock", font=("arial 24 bold"))
digi.grid(row=0, column=2)

digi_clock = Label(root, text="hours   minutes    seconds    ", font="arial 17 bold")
digi_clock.grid(row=3, column=2)


root.mainloop()


#THANKS FOR WATCHING
