

from tkinter import*
from tkinter import messagebox
import math
list=[]
r1=0
r=Tk()
e=Entry(r,bg="orange")
def a(b):
    e.insert(10,b)
    list.append(str(b))
    print(list)
    d="".join(list)
    print(d)
    
    
def b():
    s="".join(list)
    r=str(eval(s))
    print(r)
    e.delete(0,30)
    e.insert(10,r)
    list.clear()
    list.append(r)
def c():
    list.clear()
    e.delete(0,30)
def binary():
    e.delete(0,10)
    k="".join(list)
    a=int(k)
    d=[]
    x=[]
    while math.floor(a)!=0:
        r=a%2
        d.append(r)
        a=math.floor(a/2)
    while len(d)!=0:
        ele=d.pop()
        x.append(ele)
    for i in x:
        e.insert(10,i)
        list.append(str(i))
    list.clear()
def sin():
    e.delete(0,10)
    k="".join(list)
    a=int(k)
    b=math.sin(a)
    list.clear()
    e.insert(10,b)
    list.append(str(b))
def cos():
    e.delete(0,10)
    k="".join(list)
    a=int(k)
    b=math.cos(a)
    list.clear()
    e.insert(10,b)
    list.append(str(b))
def tan():
    e.delete(0,30)
    k="".join(list)
    a=int(k)
    b=math.tan(a)
    list.clear()
    e.insert(10,b)
    list.append(str(b))
def log():
    e.delete(0,30)
    k="".join(list)
    a=int(k)
    d=math.log(a)
    e.insert(10,d)
    list.clear()
    list.append(str(d))
def exp():
    e.delete(0,30)
    k="".join(list)
    print(k)
    a=int(k)
    d=math.exp(a)
    e.insert(10,d)
    list.clear()
    list.append(str(d))
def hex():
    d=[]
    x=[]
    e.delete(0,30)
    k="".join(list)
    a=int(k)
    while a!=0:
        r=a%16
        if r<10:
            d.append(r)
        else:
            if r==10:
                d.append('a')
            if r==11:
                d.append('b')
            if r==12:
                d.append('c')
            if r==13:
                d.append('d')
            if r==14:
                d.append('e')
            if r==15:
                d.append('f')
        a=math.floor(a/16)
    while len(d)!=0:
        ele=d.pop()
        x.append(ele)
    list.clear()
    for i in x:
        e.insert(10,i)
        list.append(str(i))
        
    
def oct():
    k="".join(list)
    a=int(k)
    d=[]
    x=[]
    e.delete(0,30)
    while a!=0:
        r=a%8
        d.append(r)
        a=math.floor(a/8)
    while len(d)!=0:
        ele=d.pop()
        x.append(ele)
    list.clear()
    for i in x:
        e.insert(10,i)
        list.append(str(i))
    
def btd():
     a="".join(list)
     e.delete(0,30)
     i=len(a)-1 
     sum=0
     k=0
     while i>=0:
         if a[i]=='0':
             sum=(sum+math.pow(2,k)*0)
             
         if a[i]=='1':
             sum=(sum+math.pow(2,k)*1)
         i=i-1
         k=k+1
     list.clear()    
     t=math.floor(sum)
     e.insert(10,t)
     list.append(str(t))
def l():
    r.configure(background="white")
    e.grid(columnspan=300,ipadx=220)
    
    r.geometry('560x520')
    b1.configure(background="yellow",height=6,width=12)
    b2.configure(background="yellow",height=6,width=12)
    b3.configure(background="yellow",height=6,width=12)
    b4.configure(background="yellow",height=6,width=12)
    b5.configure(background="yellow",height=6,width=12)
    b6.configure(background="yellow",height=6,width=12)
    b7.configure(background="yellow",height=6,width=12)
    b8.configure(background="yellow",height=6,width=12)
    b9.configure(background="yellow",height=6,width=12)
    b10.configure(background="yellow",height=6,width=12)
    b11.configure(background="yellow",height=6,width=12)
    b12.configure(background="yellow",height=6,width=12)
    b13.configure(background="yellow",height=6,width=12)
    b14.configure(background="yellow",height=6,width=12)
    b15.configure(background="yellow",height=6,width=12)
    b16.configure(background="yellow",height=6,width=12)
    b17.configure(background="yellow",height=6,width=12)
    b18.configure(background="yellow",height=6,width=12)
    b19.configure(background="yellow",height=6,width=12)
    b20.configure(background="yellow",height=6,width=12)
    b21.configure(background="yellow",height=6,width=12)
    b22.configure(background="yellow",height=6,width=12)
    b23.configure(background="yellow",height=6,width=12)
    b24.configure(background="yellow",height=6,width=12)
    b25.configure(background="yellow",height=6,width=12)
    b26.configure(background="yellow",height=6,width=12)
    b27.configure(background="yellow",height=6,width=12)
    b28.configure(background="yellow",height=6,width=12)
    b29.configure(background="yellow",height=6,width=12)
def n():
    r.configure(background="grey")
    r.geometry('470x300')
    b1.configure(background="white",height=3,width=10)
    b2.configure(background="white",height=3,width=10)
    b3.configure(background="white",height=3,width=10)
    b4.configure(background="white",height=3,width=10)
    b5.configure(background="white",height=3,width=10)
    b6.configure(background="white",height=3,width=10)
    b7.configure(background="white",height=3,width=10)
    b8.configure(background="white",height=3,width=10)
    b9.configure(background="white",height=3,width=10)
    b10.configure(background="white",height=3,width=10)
    b11.configure(background="white",height=3,width=10)
    b12.configure(background="white",height=3,width=10)
    b13.configure(background="white",height=3,width=10)
    b14.configure(background="white",height=3,width=10)
    b15.configure(background="white",height=3,width=10)
    b16.configure(background="white",height=3,width=10)
    b17.configure(background="white",height=3,width=10)
    b18.configure(background="white",height=3,width=10)
    b19.configure(background="white",height=3,width=10)
    b20.configure(background="white",height=3,width=10)
    b21.configure(background="white",height=3,width=10)
    b22.configure(background="white",height=3,width=10)
    b23.configure(background="white",height=3,width=10)
    b24.configure(background="white",height=3,width=10)
    b25.configure(background="white",height=3,width=10)
    b26.configure(background="white",height=3,width=10)
    b27.configure(background="white",height=3,width=10)
    b28.configure(background="white",height=3,width=10)
    b29.configure(background="white",height=3,width=10)
    

    
    
    

r.configure(background="orange")
r.geometry('470x300')
r.title("WELCOME TO ANUJ CALCULATOR")
f=Frame(r)

e.insert(10,"WELCOME")
e.grid(columnspan=300,ipadx=178)
b1=Button(r,text="1",command=lambda:a(1),height=3,width=10)
b1.grid(row=2,column=0)
b2=Button(r,text="2",command=lambda:a(2),height=3,width=10)
b2.grid(row=2,column=1)
b3=Button(r,text="3",command=lambda:a(3),height=3,width=10)
b3.grid(row=2,column=2)
b4=Button(r,text="4",command=lambda:a(4),height=3,width=10)
b4.grid(row=3,column=0)
b5=Button(r,text="5",command=lambda:a(5),height=3,width=10)
b5.grid(row=3,column=1)
b6=Button(r,text="6",command=lambda:a(6),height=3,width=10)
b6.grid(row=3,column=2)
b7=Button(r,text="7",command=lambda:a(7),height=3,width=10)
b7.grid(row=4,column=0)
b8=Button(r,text="8",command=lambda:a(8),height=3,width=10)
b8.grid(row=4,column=1)
b9=Button(r,text="9",command=lambda:a(9),height=3,width=10)
b9.grid(row=4,column=2)
b10=Button(r,text="0",command=lambda:a(0),height=3,width=10)
b10.grid(row=5,column=1)
b11=Button(r,text="enter",command=b,height=3,width=10)
b11.grid(row=5,column=0)
b12=Button(r,text="clear",command=c,height=3,width=10)
b12.grid(row=2,column=4)
b13=Button(r,text="*",command=lambda:a('*'),height=3,width=10)
b13.grid(row=3,column=4)
b14=Button(r,text="-",command=lambda:a('-'),height=3,width=10)
b14.grid(row=4,column=4)
b15=Button(r,text="/",command=lambda:a('/'),height=3,width=10)
b15.grid(row=5,column=4)
b16=Button(r,text="+",command=lambda:a('+'),height=3,width=10)
b16.grid(row=6,column=4)
b17=Button(r,text="%",command=lambda:a('%'),height=3,width=10)
b17.grid(row=6,column=2)
b18=Button(r,text="sin",command=sin,height=3,width=10)
b18.grid(row=2,column=6)
b19=Button(r,text="cos",command=cos,height=3,width=10)
b19.grid(row=3,column=6)
b20=Button(r,text="tan",command=tan,height=3,width=10)
b20.grid(row=4,column=6)
b21=Button(r,text="log",command=log,height=3,width=10)
b21.grid(row=5,column=6)
b22=Button(r,text="exp",command=exp,height=3,width=10)
b22.grid(row=6,column=6)
b23=Button(r,text="bin",command=binary,height=3,width=10)
b23.grid(row=2,column=7)
b24=Button(r,text="hex",command=hex,height=3,width=10)
b24.grid(row=3,column=7)
b25=Button(r,text="oct",command=oct,height=3,width=10)
b25.grid(row=4,column=7)
b26=Button(r,text="btd",command=btd,height=3,width=10)
b26.grid(row=4,column=7)
b27=Button(r,text=".",command=lambda:a('.'),height=3,width=10)
b27.grid(row=5,column=2)
b28=Button(r,text="(",command=lambda:a('('),height=3,width=10)
b28.grid(row=6,column=0)
b29=Button(r,text=")",command=lambda:a(')'),height=3,width=10)
b29.grid(row=6,column=1)
m=Menu(r)
r.config(menu=m)
f=Menu(m)
m.add_cascade(label="|||",menu=f)
f.add_command(label="changecolor",command=l)
f.add_command(label="neutralise",command=n)




   
    
    

