import robloxpy
from robloxpy import Group
import tkinter as tk

RoGUI1 = tk.Tk()
RoGUI1.title("Roblox Group Shower")

Te_xt = tk.Label(RoGUI1, text="")
Te_xt.pack()

Label_1 = tk.Label(RoGUI1, text="")
Label_1.pack()

Desc = tk.Label(RoGUI1, text="")
Desc.pack()

RoGUI = tk.Tk()
RoGUI.title("Roblox Group Input")

Text_Overview = tk.Label(RoGUI, text="Input Group ID")
Text_Overview.pack()

Entry = tk.Entry(RoGUI)
Entry.pack()


def Get_Name():
    GroupName = Group.External.GetName(Entry.get())
    GetDesc = Group.External.GetDescription(Entry.get())
    GetOwner = Group.External.GetOwner(Entry.get())

    Te_xt.config(text="Group Name: "+GroupName)
    Label_1.config(text="Group Owner: "+GetOwner)
    Desc.config(text="Description: "+GetDesc)

    RoGUI.destroy()


Button = tk.Button(RoGUI, text="Enter", command=Get_Name)
Button.pack()

RoGUI.mainloop()

RoGUI1.mainloop()



