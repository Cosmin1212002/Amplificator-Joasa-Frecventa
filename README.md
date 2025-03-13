# Amplificator-Joasa-Frecventa
  Pentru acest amplificator am utilizat o reacție serie-paralel, obținând o amplificare  ridicată în buclă deschisă. Designul asigură o impedanță de intrare mare și o impedanță de ieșire  foarte mică, fiind realizat cu tranzistoare bipolare.

  Alimentarea in curent a circuitului se realizeaza astfel: rezistenta R7 si R18, pe care aplic 
tensiune . Curentul acesta e preluat de Q14 si transmis prin circuit prin Q18 si Q19 care 
impreuna cu tranzistorul Q14 formeaza oglinzi de curent. Rezistentele R7 si R18 au fost 
dimensionate astfel incat sa am prin ele un curent de aproximativ 0.7 mA. 

  Partea de amplificator e reprezentata de Q15 si Q20 tranzistoare de intrare, pereche 
diferentala. Unul va fi intrarea inversoare si unul intrarea neinversoare. Tranzistoarele Q9 si Q10 
reprezinta sarcina pentru etajul de intrare si totodata au rolul (fiind in configurate de oglinda de 
curent) sa tina curentii pe cele 2 ramuri de intrare, egali.  

  Mai departe avem etajul de castig Q12, etaj de tipul emitor-comun, care are si un 
condensator Miller de compensare in frecventa (muta polul dominant mai la dreapta, obtine o 
rezerva de faza buna). Q12 asta si intrarea sunt principalele stagii de amplificare. 

  Din tranzistorul de castig, semnalul merge mai departe spre sarcina (iesirea). Pentru etajul 
de iesire am utilizat un etaj de iesire clasa AB (tranzistoarele Q4 si Q17), pereche push-pull(cand 
vine in acest etaj semnalul amplificat anterior, pe alternantata pozitva va fi deschis NPN-ul iar pe 
negative, PNP-ul. Mereu fiind unul blocat, nu exista consum de curent static intre VCC si VEE). 
E clasa AB pentru ca perechea asta e prepolarizata cu 2 diode (Q7 si Q16) in configuratie de 
dioda, care asigura un Vbe aproape constant pe cele 2 tranzistoare de iesire (ca sa avem 0.6 pe 
fiecare dioda, trebuie trecut un curent prin ea, de aceea avem nevoie de oglinda de sus). R3 si R5 
de 1 ohm sunt rezistente de protectie. 

  Intre intrare si iesire am pus o reactie negativa serie-paralel (e negativa pentru ca se 
intoarce pe intrarea negativa a amplificatorului), o retea rezistiva de 9.1k si 1k. Dupa calculul de 
AC pe retea avem f = 1k/(9k+1k). Adica f=1/10. Cum amplificarea in bucla deschisa e foarte 
mare (pe masurate) undeva la 8-9000x, amplificarea totala o sa ramana 1/f adica 10.
