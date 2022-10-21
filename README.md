# Pr_001
- Programmeerimise õpik - https://progeopik.cs.ut.ee/01_sissejuhatus.html  
- KÜSIME 2 TÄISARVU JA TEEME 7 PÕHILIST ARITMEETILIST TEHET  
- Seotud: Alg_001  
![Alg_001](https://user-images.githubusercontent.com/115221752/197119739-80afe7b7-6d8a-4399-afe8-798e29f81e6b.JPG)

`print("Esimene arv ")`  
- Kuvab teksti ekraanile  
`arv1=int(input())`  
- arv1=input("Esimene arv ")   Saab ka nii(esimesed read kokku)  
- INT teisendab sisestatud teksti numbriks  

`arv2=int(input("Teine arv "))`  
- Kasutatud lühendatud varianti  
- Kui ei kasuta INT varianti, siis error... teksti ja numbrit ei saa liita  

`arv3=arv1+arv2`  

`print("Summa = ",arv3)`  

- Alternatiivid  
`print("Summa = ",arv1+arv2)`  
`print(arv1, "+", arv2, "=",arv1+arv2)`  

- 7 põhilist aritmeetilist tehet  
- "," sümboliseerib + märki  
```
print(arv1, "+", arv2, "=",arv1+arv2)
print(arv1, "-", arv2, "=",arv1-arv2)
print(arv1, "x", arv2, "=",arv1*arv2)
print(arv1, ":", arv2, "=",arv1/arv2)
print(arv1, "Täisarvuline jagamine", arv2, "=",arv1//arv2)   - Mitu korda mahub arv 2 esimesse arvu  
print(arv1, "Jääk", arv2, "=",arv1%arv2)   - Kui arv 2 mahub, siis palju üle jääb  
print(arv1, "Aste", arv2, "=",arv1**arv2)
```

# Pr_002
- KÜSIME 2 TÄISARVU JA LEIAME KUMB ARV ON SUUREM JA MIS ON NEDE MAKSIMUM VÄÄRTUS  
- Seotud: Alg_002  
![Alg_002](https://user-images.githubusercontent.com/115221752/197119812-0effe90b-013a-4d88-8d60-52b3c4a8d719.JPG)

```
arv1=int(input("Esimene arv "))
arv2=int(input("Teine arv "))
```
- Kas esimene arv on suurem?  
```
if (arv1>arv2):
    print("Esimene arv on suurem!")
```    
- Aga kui ei ole... kas teine arv on suurem või on need võrdsed  
- Blokkide liigendus peab olema õige  
```
else:
    if(arv2>arv1):
        print("Teine arv on suurem!")
    else:
        print("Sisestatud arvud on võrdsed!")
```

- Lihtsustatud variant  
- Jälgi liigendusi!  
```
if (arv1>arv2):
    print("Esimene arv on suurem!")
elif(arv2>arv1):
    print("Teine arv on suurem!")
else:
    print("Sisestatud arvud on võrdsed!")
```    
- Leiame sisestatud arvude maksimaalse väärtuse
```
if (arv1>arv2):
    print("Maksimum on",arv1)
elif(arv2>arv1):
    print("Maksimum on",arv2)
else:
    print("Maksimum on",arv1)
```

# Pr_003
- KÜSIME 3 TÄISARVU JA LEIAME NENDE MAKSIMAALSE VÄÄRTUSE  
- Seotud: Alg_003  
![Alg_003](https://user-images.githubusercontent.com/115221752/197119860-68303c1a-7184-453f-9b76-696add9d05e5.JPG)

```
arv1=int(input("Esimene arv "))
arv2=int(input("Teine arv "))
arv3=int(input("Kolmas arv "))

if (arv1>=arv2):
    if(arv1>=arv3):
        print("Maksimum =",arv1)
    else:
        print("Maksimum =",arv3)    
else:
    if(arv2>=arv3):
        print("Maksimum =",arv2)
    else:
        print("Maksimum =",arv3)
```

# Pr_004
- 3 loogilist tehet (AND, OR, NOT)
- LOOGILINE KORRUTIS (AND) - LEIAME 3 TÄISARVU MAKSIMUMI
- Seotud: Alg_004  
![Alg_004](https://user-images.githubusercontent.com/115221752/197122889-f7c29c68-d064-4685-9195-1b1310763b73.JPG)

```
arv1=int(input("Esimene arv "))
arv2=int(input("Teine arv "))
arv3=int(input("Kolmas arv "))

if (arv1>=arv2 and arv1>=arv3):
    maksimum=arv1    
elif(arv2>=arv3):
    maksimum=arv2
else:
    maksimum=arv3
print("Maksimum =",maksimum)
```

# Pr_005
- LEIAME IGA JÄRGNEVA TÄISARVU HULGAST MAKSIMUMI
- Seotud: Alg_005  

```
arv1=int(input("Esimene arv "))
arv2=int(input("Teine arv "))
arv3=int(input("Kolmas arv "))
maksimum=arv1
if (arv2>=maksimum):
    maksimum =arv2
if (arv3>=maksimum):
    maksimum =arv3
print("Maksimum =",maksimum)
```

# Pr_006
- KORDUSLAUSED, MIS OTSIVAD MAKSIMUMI
- Seotud: Alg_006  
![Alg_006](https://user-images.githubusercontent.com/115221752/197129691-e30717d3-719f-4d95-a804-0559385e15f0.JPG)

```
arv=int(input("Sisesta esimene arv "))
maksimum=arv
loendur=2
while(loendur<=5):
    arv=int(input("Sisesta järgmine arv "))
    if(arv>maksimum):
        maksimum=arv
    loendur+=1   ## Sama, mis loendur=loendur+1
print("Maksimum =",maksimum)
```

# Pr_007
- KORDUSLAUSED, MIS OTSIVAD MAKSIMUMI
- Seotud: Alg_007  


```
arv=int(input("Sisesta esimene arv "))
maksimum=arv
loendur=2
while(loendur<=5):
    arv=int(input("Sisesta järgmine arv "))
    if(arv>maksimum):
        maksimum=arv
    loendur+=1   ## Sama, mis loendur=loendur+1
print("Maksimum =",maksimum)
```
