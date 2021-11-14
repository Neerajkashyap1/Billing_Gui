# Billing_Gui
import turtle
from tkinter import *
window=Tk()
window.geometry("850x500")
def calculator():                                       #creatin calc fn
    Coffee=e1.get()
    Sandwich=e2.get()                                   #e.get fn to extract the value
    Muffins=e2.get()
    Fried_rice=e3.get()
    Aalu_Paratha=e4.get()
    Tea=e5.get()
    Spring_roll=e6.get()
    Samosa=e7.get()
    total=((int(Aalu_Paratha)*50)+(int(Sandwich)*50)+(int(Coffee)*20)+(int(Muffins)*40)+(int(Fried_rice)*80)+(int(Tea)*20)+(int(Spring_roll)*20)+(int(Samosa)*30))
    label18 = Label(window, text=total, font="times 18")             #here window is gui class
    label18.place(x=110, y=380)

label7=Label(window,text="DEMO RESTAURANT",font="times 38 bold")
label7.place(x=420,y=20,anchor="center")

#menu section

label1=Label(window,text="MENU :)",font="times 28 bold")
label1.place(x=550,y=80)                                                            #labels using function

label2=Label(window,text="Coffee                    20Rs",font="times 18")
label2.place(x=550,y=130)

label4=Label(window,text="Sandwich               50Rs",font="times 18")
label4.place(x=550,y=160)

label5=Label(window,text="Muffins                  40Rs",font="times 18")
label5.place(x=550,y=190)

label6=Label(window,text="Aaalu Paratha        50Rs",font="times 18")
label6.place(x=550,y=220)

label7=Label(window,text="Tea                         20Rs",font="times 18")
label7.place(x=550,y=250)

label8=Label(window,text="Spring Rolls            20Rs",font="times 18")
label8.place(x=550,y=280)

label9=Label(window,text="Samosa                   30Rs",font="times 18")
label9.place(x=550,y=310)

label10=Label(window,text="Fried Rice               80Rs",font="times 18")
label10.place(x=550,y=340)

#------------Billing Section----------------#

label12=Label(window,text="     Select the items     ",font="times 20 bold")
label12.place(x=70,y=80)

label13=Label(window,text="Coffee",font="times 18")
label13.place(x=20,y=120)
e1=Entry(window)
e1.place(x=20,y=150)

label14=Label(window,text="Sandwich",font="times 18")
label14.place(x=20,y=180)
e2=Entry(window)
e2.place(x=20,y=210)

label15=Label(window,text="Muffins",font="times 18")
label15.place(x=20,y=240)
e3=Entry(window)
e3.place(x=20,y=270)

label16=Label(window,text="Fried Rice",font="times 18")
label16.place(x=20,y=300)
e4=Entry(window)
e4.place(x=20,y=330)

label17=Label(window,text="Aaalu Paratha",font="times 18")
label17.place(x=250,y=120)
e5=Entry(window)                                        #e entry widget
e5.place(x=250,y=150)

label18=Label(window,text="Tea",font="times 18")
label18.place(x=250,y=180)
e6=Entry(window)
e6.place(x=250,y=210)

label19=Label(window,text="Spring Rolls",font="times 18")
label19.place(x=250,y=240)
e7=Entry(window)
e7.place(x=250,y=270)

label18=Label(window,text="Samosa",font="times 18")
label18.place(x=250,y=300)
e8=Entry(window)
e8.place(x=250,y=330)

b2=Button(window,text='BILL',width=20,command=calculator)
b2.place(x=120,y=380)

window.mainloop()
