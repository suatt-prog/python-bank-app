from tkinter import *
root=Tk()
root.title("TOPCU BANKACILIK")
sifre=Entry(root,width=70,bg="red")
sifre.grid(row=1)
global y
def donus():
    v=root.winfo_children()
    for i in v:
       i.destroy()
    gir1=Button(root,padx=400,pady=40,text="BAKİYE KONTROL",command=bakiye).grid(row=0,columnspan=3)
    cek=Button(root,padx=400,pady=40,text="PARA ÇEK",command=ceki).grid(row=1,columnspan=3)
    yatir=Button(root,text="PARA YATIR",padx=400,pady=40,command=yati).grid(row=2)
def yat1():
    global bakiy
    bakiy=int(1350)
    global miktar
    global y
    miktar=int(y.get())
    bakiy=bakiy+miktar
    e=root.winfo_children()
    for q in e:
        q.destroy()
    p=Label(root,text="Yeni bakiyeniz: "+str(bakiy),bg="#355668",width=30,height=10).grid(row=0)
    k=Button(root,text="GERİ",command=donus,padx=50,pady=50,bg="green").grid(row=1)
def yati():
    global bakiy
    e=root.winfo_children()
    for q in e:
        q.destroy()
    global y
    r=Label(root,text="Lütfen yatırmak istediğiniz miktarı girin",width=30,height=7).grid(row=0)
    y=Entry(root,width=40)
    y.grid(row=1)
    bu=Button(root,padx=50,pady=50,command=yat1,bg="black",fg="white",text="Gir").grid(row=2,column=2)
    k=Button(root,text="GERİ",command=donus,padx=50,pady=50,bg="green").grid(row=3)
def cek1():
    global bakiy
    bakiy=int(1350)
    global miktar
    global y
    miktar=int(y.get())
    bakiy=bakiy-miktar
    e=root.winfo_children()
    for q in e:
        q.destroy()
    p=Label(root,text="Yeni bakiyeniz: "+str(bakiy),bg="#355668",width=30,height=10).grid(row=0)
    k=Button(root,text="GERİ",command=donus,padx=50,pady=50,bg="green").grid(row=1)
def ceki():
    global bakiy
    e=root.winfo_children()
    for q in e:
        q.destroy()
    global y
    r=Label(root,text="Lütfen çekmek istediğiniz miktarı girin",width=30,height=7).grid(row=0)
    y=Entry(root,width=40)
    y.grid(row=1)
    bu=Button(root,padx=50,pady=50,command=cek1,bg="black",fg="white",text="Gir").grid(row=2,column=2)
    k=Button(root,text="GERİ",command=donus,padx=50,pady=50,bg="green").grid(row=3)
def bakiye():
    global bakiy
    bakiy=int(1350)
    liste=root.winfo_children()
    for i in liste:
        i.destroy()
    bak=Label(root,text="Şuanki bakiyeniz: "+str(bakiy),padx=200,pady=100,bg="red",fg="white").grid(row=0,column=0)
    k=Button(root,text="GERİ",command=donus,padx=50,pady=50,bg="green").grid(row=1)
def girf():
    global a
    a=sifre.get()
    if sifre.get()=="6169":
       yazi.grid_forget()
       sifre.grid_forget()
       sad=root.winfo_children()#ÖNEMLİ
       for t in sad:
           t.destroy()
       gir1=Button(root,padx=400,pady=40,text="BAKİYE KONTROL",command=bakiye).grid(row=0,columnspan=3)
       cek=Button(root,padx=400,pady=40,text="PARA ÇEK",command=ceki).grid(row=1,columnspan=3)
       yatir=Button(root,text="PARA YATIR",padx=400,pady=40,command=yati).grid(row=2)
    else:
        sifre.delete(0,END)
yazi=Label(root,text="Şifrenizi giriniz",bg="orange")
yazi.grid(row=0,columnspan=3)
gir=Button(root,text="Gir",command=girf,padx=50,pady=30).grid(row=2,column=1,columnspan=2)
root.mainloop()
