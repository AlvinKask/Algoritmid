# Pr_001
- Programmeerimise õpik - https://progeopik.cs.ut.ee/01_sissejuhatus.html  
- KÜSIME 2 TÄISARVU JA TEEME 7 PÕHILIST ARITMEETILIST TEHET  
- Seotud: Alg_001  

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
