from tkinter import*
from tkinter import messagebox
from tkinter import ttk
import pymysql
#-------------------------------------end the head---------------------------------------------
#---------------------------------end vars-----------------------------------------------------
login=Tk()
login.geometry('600x300')
login.resizable(False,False)                
login.title("ADHAM")
lab=Label(login, text="تسجيل دخول", height=2, font=( "Arial",20))
lab.pack()
name=StringVar()
name1=StringVar()
name_input=Entry(login, width=30, font=("Arial",15),  textvariable=name)
name_input.pack()
lab2=Label(login, text="", height=1, font=( "Arial",15) ) 
lab2.pack()
name_input1=Entry(login, width=30, font=("Arial",15), textvariable = name1)
name_input1.pack()
lab3=Label(login,text=" ",height=1, font=( "Arial",20))
lab3.pack()
login.quit

#-------------------------------------end login----------------------------------------------
def man():
    xxc=name.get()
    xxc1=name1.get()
    admins= ('adham')
    password= ("12345")
    serial=("jbihijhws758hdxxxx")
    number1=("01100609036")
    verision=(1.3)
    if xxc1 != password or xxc != admins  :
      messagebox.showinfo(f"error", {xxc})
      print(name.get())
      print(xxc1)
      def add():
       con=pymysql.connect(host='localhost',user='root',password='',database='adham')
       cur=con.cursor()
       cur.execute("insert into vvc values(%s,%s,%s)",(name.get(),name1.get(),555))
       con.commit()
       con.close()
      



      
 #---------------------------------------end fun the login-------------------------------------     
    elif xxc1  == password or xxc==admins :
     ffg=Tk()
     ffg.geometry("1350x1200")
     ffg.configure(background='#F5F5DC') 
    
     macframe=Frame(ffg,bg='#A8A8FF')
     macframe.place(x=0,y=2, width=1350, height=35)
     start=Button(macframe,text='اضافه عميل', width=20,bg='#F5F7FE', border=0, command=client).place(x=10,y=4)
     start=Button(macframe,text='تعديل بيانات', width=20, border=0).place(x=210,y=4)
     start=Button(macframe,text='عملاء انتهوا', width=20, border=0).place(x=410,y=4) 
     start=Button(macframe,text='عملاء لم ينتهوا', width=20, border=0).place(x=610,y=4)
     def woman ():
      messagebox.showinfo("من نحن","شركه KHEDMAH ONLINEشركه لحل جميع المشاكل الالكترونيه وانشاء المواقع والتطبيقات للتواصل معنا: xxxxxxxxxxx")
     start=Button(macframe,text=' من نحن', width=20, border=0 ,command=woman).place(x=810,y=4)
     macframe3=Frame(ffg,bg='black')
     macframe3.place(x=0,y=910, width=1330, height=250)
     macframe4=Frame(ffg,bg='#A8A8FF')
     macframe4.place(x=-25,y=1170, width=1350, height=40)
     lab4=Label(macframe4,text=f"{admins} الاسم",height=1, font=( "Arial",15),fg='black', bg='#A8A8FF',)
     lab4.place(x=35,y=4)
     lab5=Label(macframe4,text=f"{number1} رقم التليفون",height=1, font=( "Arial",15),fg='black', bg='#A8A8FF')
     lab5.place(x=230,y=4)
     lab6=Label(macframe4,text=f"{serial} السريال",height=1, font=( "Arial",15),fg='black', bg='#A8A8FF')
     lab6.place(x=530,y=4)
     lab7=Label(macframe4,text=f"{verision} الاصدار",height=1, font=( "Arial",15),fg='black', bg='#A8A8FF')
     lab7.place(x=880,y=4)
     lab8=Label(macframe3,text="CREATOR BY: KEDMAH ONLINE",font=( "Arial",15),fg='white', bg='black')
     lab8.place(x=0,y=210)
     #lab9=Label(macframe3,text="It is a new type of accounting program in which the trader does not contact the customer with all sohohelham are the benefits of the program: customer account and late month account in payment of the premium interest account and save customers and more within the name of the programs",font=( "Arial",20),fg='white', bg='black',height=1,)
     #lab9.place(x=0,y=210)                                              
     ffg.mainloop() 
ooo1 =StringVar() 
ooo2 =StringVar()
ooo3 =StringVar()
ooo4 =StringVar()
     
#--------------------------------------------------end ffg--------------------------------------   

btn=Button(login,text="login", width=20, height=2, 
bg="#e91e63", fg="white", borderwidth=0,)
btn.place(x=310,y=190)

def ooo ():
   ffo=Tk()
   ffo.geometry("600x600")
   ffo.resizable(False,False)
   ffo.title("ADHAM")
   ccv1=Label(ffo,text="الايميل", font=("Arial",15),height=2,fg='black', )
   ccv1.pack()
   ccv1.pack()
   ooo1_input=Entry(ffo, width=30, font=("Arial",15),textvariable=ooo1)
   ooo1_input.pack()
   ccv2=Label(ffo,text=" ", font=("Arial",15),fg='black', )
   ccv2.pack()


   ccv2=Label(ffo,text="الباسورد", font=("Arial",15),height=2,fg='black', )
   ccv2.pack()
   ooo2_input=Entry(ffo, width=30, font=("Arial",15),  textvariable=ooo2)
   ooo2_input.pack()
   ccv2=Label(ffo,text=" ", font=("Arial",15),fg='black', )
   ccv2.pack()


   ccv3=Label(ffo,text=" اسم الشخص او المنشائه  ", font=("Arial",15),height=2,fg='black', )
   ccv3.pack()
   ooo3_input=Entry(ffo, width=30, font=("Arial",15),  textvariable=ooo3)
   ooo3_input.pack()
   ccv2=Label(ffo,text=" ", font=("Arial",15),fg='black', )
   ccv2.pack()


   ccv4=Label(ffo,text="السريال", font=("Arial",15),height=2,fg='black', )
   ccv4.pack()
   ooo4_input=Entry(ffo, width=30, font=("Arial",15),  textvariable=ooo4)
   ooo4_input.pack()
   ccv2=Label(ffo,text=" ", font=("Arial",15),fg='black', )
   ccv2.pack()


   ccv2=Label(ffo,text=" ", font=("Arial",15),fg='black', )
   ccv2.pack()
  
  # def add():
      # con=pymysql.connect(host='localhost',user='root',password='',database='adham')
     #  cur=con.cursor()
      # cur.execute("insert into vvc values(%s,%s,%s)",(ooo1.get(),ooo2.get(),555))
       #con.commit()
     #  con.close()

   


   
  
    
   ccv5=Button(ffo,text="sing in",width=40,bg="#e91e63", height=2,fg="white", 
   borderwidth=0,)   
   ccv5.pack()
   ffo.mainloop()

beur=Button(login,text="hhhh",width=20,bg="#e91e63", height=2,fg="white", borderwidth=0,command=ooo )   
beur.place(x=150,y=190)

# # #-----------------------------------------------end butt and fun the login------------------------

def client ():
   client=Tk()
   client.geometry('1300x1400')
   client.configure(background='#F5F5DC')
   #.resizable(False,False)                
   client.title("ADHAM")
   wwe=StringVar()
   wwe1=StringVar()
   wwe2=StringVar()
   wwe3=StringVar()
   wwe4=StringVar()
   wwe5=StringVar()
   wwe6=StringVar() 
  
   oap1=Label(client,text="الاسم",height=3, font=( "Arial",15),fg='black', bg='#F5F5DC',)
   oap1.pack()
   wwe_input=Entry(client,width=40,font=("Arial",15),textvariable=wwe )
   wwe_input.pack()


   oap2=Label(client,text=" الرقم القومي  ",height=3, font=( "Arial",15),fg='black', bg='#F5F5DC',)
   oap2.pack()
   wwe1_input=Entry(client,width=40,font=("Arial",15),textvariable=wwe1 )
   wwe1_input.pack()


   oap3=Label(client,text="عدد الشهور ",height=3, font=( "Arial",15),fg='black', bg='#F5F5DC',)
   oap3.pack()
   wwe2_input=Entry(client,width=40,font=("Arial",15),textvariable=wwe2 )
   wwe2_input.pack()


   oap4=Label(client,text="السعر ",height=3, font=( "Arial",15),fg='black', bg='#F5F5DC',)
   oap4.pack()
   wwe_3input=Entry(client,width=40,font=("Arial",15),textvariable=wwe3 )
   wwe_3input.pack()


   oap5=Label(client,text="نوع ",height=3, font=( "Arial",15),fg='black', bg='#F5F5DC',)
   oap5.pack()
   wwe4_input=Entry(client,width=40,font=("Arial",15),textvariable=wwe4 )
   wwe4_input.pack()

   oap6=Label(client,text="الفايده",height=3, font=( "Arial",15),fg='black', bg='#F5F5DC')
   oap6.pack()
   wwe5_input=Entry(client,width=40,font=("Arial",15),textvariable=wwe5 )
   wwe5_input.pack()

   oap7=Label(client,text=" الرقم القومي 2",height=3, font=( "Arial",15),fg='black', bg='#F5F5DC',)
   oap7.pack()
   wwe6_input=Entry(client,width=40,font=("Arial",15),textvariable=wwe6 )
   wwe6_input.pack()

   pll=Button(client,text="submit",width=40,bg="#e91e63", height=2,fg="white", 
   borderwidth=0,)   
   pll.pack()


#--------------------------------------end the clients-------------------------------------








#-----------------------------------------end insert----------------------------------------
login.mainloop()
#users (email,password,shop)
