import random
reci2=[]
reci1=[]
lista1=['','','']  #ovde se unose reci koje treba da se prevedu
lista2=['','','']   #ovde se unosi potreban prevod
lista=list(zip(lista1,lista2))
random.shuffle(lista)
for i in lista:
    reci1.append(i[0])
    reci2.append(i[1])

i=0
broj_reci = len(reci1)
rezultat=1
broj_nepogodjenih_reci=0
while i<broj_reci:
    print(reci1[i],end=' : ')
    x=input()
    if x==reci2[i]:
        print('Tacno')
        i += 1
        rezultat += 1

    elif x=='dalje':
        i+=1

    else:
        print('Netacno')
        rezultat -=1
        if rezultat < 0:
            i+=1
            broj_nepogodjenih_reci+=1


if broj_nepogodjenih_reci==0:
    print("Sve reci su pogodjene")

else:
    print("Broj nepogodjenih reci je:",broj_nepogodjenih_reci," od ukupno ",broj_reci," reci ")

print("Rezultat je: ",rezultat-1)

print('Procenat tacnosti: ',((rezultat-1)/broj_reci)*100,'%')
