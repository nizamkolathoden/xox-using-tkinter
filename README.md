# **Tick Tack Toe**

we developed a Simpale **Tick Tack Toe** Desktop game

## installation

* ### **python** 
    Click here to download [python3](https://www.python.org/downloads/)

*  ### **pip** 
Open cmd then type

      python get-pip.py

*  ### **Tinker** 
Open cmd then type

        pip install tk

### **Pre-requisites:**

    Python3, pip,Tinker

### **Approch**
* Tinker  is implemented for GUI

### **Code**

```zsh
from tkinter import *

from tkinter import messagebox

window = Tk()

#window size

window.geometry("500x500")

#Title Of Game

window.title("XOX")

#Equely Dived Window 

row_1 = Frame(window,bg="#fff",)
row_1.pack(expand=True,fill="both")

row_2 = Frame(window)
row_2.pack(expand=True,fill="both",)

row_3 = Frame(window,bg="#fff",)
row_3.pack(expand=True,fill="both")
click = True
def logic(buttons):
    
    global click
    
    #cheaking

    if buttons["text"]=="" and click==True:
        buttons["text"]="X"
        click = False 
        

    elif buttons["text"]=="" and click==False:
        buttons["text"]="O"
        click = True
        
    if(btn_1["text"]=="O" and btn_2["text"]=="O" and btn_3["text"]=="O" or
    btn_4["text"]=="O" and btn_5["text"]=="O" and btn_6["text"]=="O" or
    btn_7["text"]=="O" and btn_8["text"]=="O" and btn_9["text"]=="O" or
    btn_1["text"]=="O" and btn_5["text"]=="O" and btn_9["text"]=="O" or
    btn_1["text"]=="O" and btn_7["text"]=="O" and btn_4["text"]=="O" or
    btn_5["text"]=="O" and btn_2["text"]=="O" and btn_8["text"]=="O" or
    btn_9["text"]=="O" and btn_6["text"]=="O" and btn_3["text"]=="O" or 
    btn_3["text"]=="O" and btn_5["text"]=="O" and btn_7["text"]=="O"):

         messagebox.showinfo("Winner O", "Player 2 You Have Just Won The Game")
         
         exit()

    if (btn_1["text"]=="X" and btn_2["text"]=="X" and btn_3["text"]=="X" or 
    btn_4["text"]=="X" and btn_5["text"]=="X" and btn_6["text"]=="X" or 
    btn_7["text"]=="X" and btn_8["text"]=="X" and btn_9["text"]=="X" or 
    btn_1["text"]=="X" and btn_5["text"]=="X" and btn_9["text"]=="X" or 
    btn_1["text"]=="X" and btn_7["text"]=="X" and btn_4["text"]=="X" or 
    btn_5["text"]=="X" and btn_2["text"]=="X" and btn_8["text"]=="X" or 
    btn_9["text"]=="X" and btn_6["text"]=="X" and btn_3["text"]=="X" or 
    btn_3["text"]=="X" and btn_5["text"]=="X" and btn_7["text"]=="X"):
            
        messagebox.showinfo("Winner X", "Player 1 You Have Just Won The Game")            

        exit()

#Button Designed

btn_1=Button(
    row_1,
    command=lambda:logic(btn_1)

)
btn_1.pack(side=LEFT,

expand=True,

fill="both",
)

btn_2=Button(
    row_1,
    command= lambda:logic(btn_2)
    )
btn_2.pack(side=LEFT,expand=True,fill="both",)

btn_3=Button(row_1,command=lambda:logic(btn_3))
btn_3.pack(side=LEFT,expand=True,fill="both")

btn_4=Button(row_2,command=lambda:logic(btn_4))
btn_4.pack(side=LEFT,expand=True,fill="both")

btn_5=Button(row_2,command=lambda:logic(btn_5))
btn_5.pack(side=LEFT,expand=True,fill="both")

btn_6=Button(row_2,command=lambda:logic(btn_6))
btn_6.pack(side=LEFT,expand=True,fill="both")

btn_7=Button(row_3,command=lambda:logic(btn_7))
btn_7.pack(side=LEFT,expand=True,fill="both")

btn_8=Button(row_3,command=lambda:logic(btn_8))
btn_8.pack(side=LEFT,expand=True,fill="both")

btn_9=Button(row_3,command=lambda:logic(btn_9))
btn_9.pack(side=LEFT,expand=True,fill="both")

window.mainloop()


```

### **Run code**

Open cmd then type
        
        python xox.py

### **Screenshot**

![1](https://user-images.githubusercontent.com/59057736/137676536-75eb8495-b6f1-418d-809d-75f17d753ea6.png)

![2n](https://user-images.githubusercontent.com/59057736/137676808-53476329-9606-4b63-883f-5688f6861b00.png)

![4n](https://user-images.githubusercontent.com/59057736/137676950-b86d3b36-16fd-4aee-a565-5dd9bc02298f.png)

![3n](https://user-images.githubusercontent.com/59057736/137677021-8a5560d7-c519-4a11-908a-522e3947a8a3.png)


