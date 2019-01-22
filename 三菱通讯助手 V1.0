#-*coding:utf-8-*-
from tkinter import *
app = Tk()
app.title ('三菱通讯助手')
app.geometry ('290x550')
app.resizable (width = False , height = False)
def Transform(self):
    t.delete(0.0 , END)
    strlist = list(input.get())
    strlen = len(strlist)
    a = 0
    while a < strlen:
        strlist[a] = hex(ord(strlist[a]))
        a += 1
    b = 0
    while b < strlen:
        strlist[b] = strlist[b][2:].upper()
        b += 1
    strlist1 = strlist[:]
    if strlen%2 == 0:
        pass
    else:
        strlist1.append('16#')
    strlen1 = len(strlist1)
    c = 0
    while c < strlen1:
        strlist1[c+1] += strlist1[c]
        strlist1[c] = '16#'
        strlist1[c] += strlist1[c+1]
        c += 2
    strlen2 = strlen1/2
    d = 1
    while d <= strlen2:
        del strlist1[d]
        d += 1
    if strlen%2 == 0:
        pass
    else:
        strlist1[-1] = strlist1[-1][3:]
    strlist1.append('长度:')
    strlist1.append(str(strlen))
    strlist1[-2] += strlist1[-1]
    del strlist1[-1]
    strlen3 = len(strlist1)
    e = 0
    while e < strlen3:
        t.insert(END , strlist1[e])
        t.insert(END , "\n")
        e += 1
Label(app , text = '字符串输入' , font = ('Consolas')).pack()
input = StringVar()
Entry(app , textvariable = input , width = 30 , font = ('Consolas')).pack()
Label(app , text = '转换结果' , font = ('Consolas')).pack()
t = Text(app , width = 15, font = ('Consolas')) 
t.pack()
app.bind('<Key>', Transform)
app.mainloop()
