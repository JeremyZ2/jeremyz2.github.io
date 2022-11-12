---
layout: post
title: >
    Design Game on
tags: [Test, Keystone]
---
# **Code**
## **Timer**

```Python
import time
#define
global current_time
global year
starttime = 0
year = 0
#define function
def Year(x):
    setTime = x

    starttime = time.time()
    #record current time
    while True:
        current_time = round(time.time() - starttime)
        print(current_time, " sec")
        year = round(0.2 * current_time)
        print(year," year")
        #stop the timer
        if current_time == setTime:
            break

#output
print("timer initialized")
```

## **Name record**

```Python
import tkinter as tk
window = tk.Tk()

window.title("Please name your world")
window.geometry("400x240")
textExample=tk.Text(window, height=10)

textExample.pack()
def getTextInput():
    global result
    result=textExample.get("1.0","end")    #get the inputed text
    print("This world is called " + result)
getTextInput()

btnRead = tk.Button(window, height=1, width=30, text="Click here and close this window", command=getTextInput)  # link the button
Name_des = tk.Button(window, height=2, width=30, text="You may choose to skip this step, just close this window", command=getTextInput)
    # placed button
btnRead.pack()  # display button

    # 第9步，
window.mainloop()
```