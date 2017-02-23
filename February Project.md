1. Regamine

1. Kasutajad-huvid: Kõik kasutajad. Tahavad ennast süsteemis registreerida. 

2. Primaarne kasutaja (kui on):

3. Üleüldine kirjeldus: Läbi facebooki, google’i, linkedin API’i VÕI registeerib manuaalselt. Selleks on alustuseks vaja emaili. Sisestatakse landing page’l.

4. Infovaade (kus toimub protsess): 

    1. sign up view (punkt 13.2) 

    2. sealt edasi spetsiaalsed vaated täiendava info küsimiseks.

5. Käivitav sündmus: subjekt soovib registreerida

6. Eeltingimused: kasutajal on olemas isiklik email VÕI sotsiaalmeedia konto

7. Järeltingimused: kasutaja on registeeritud, avatakse library vaade.

8. Erinõudmised: 

9. UX-UI tips:

10. UML,mockupid

11. Näited: 

    3. slack.com

    4. [https://blog.hubspot.com/marketing/landing-page-examples-list#sm.00018tqvatadsfkeynp27kz3a2wol](https://blog.hubspot.com/marketing/landing-page-examples-list#sm.00018tqvatadsfkeynp27kz3a2wol)

12. Kasutusjuhu esinemissagedus*:* igapäevaselt

13. Stsenaarium:

    5. Subjekt soovib ennast registeerida landing page’il, vajutades "sign up" nupule.

    6. Süsteem pakub valikut, kas registeerida API’de kaudu või emaili kaudu. (sign up view)

    7. Kasutaja valib emaili teel regamise, sisestades emaili.

    8. Systeem kontrollib, et email poleks eelnevalt võetud. (võimalik, et vaja lisada funktsioon, mis kontrollib, et kasutaja poleks robot).

        1. Kui email on olemas, siis systeem annab teate, et kasutaja on antud emailiga on juba olemas.

    9. Kasutajale saadetakse süsteemi poolt geneeritud 6-kohaline kood emailile.

    10. Süsteem palub sisestada kasutajale saadetud 6-kohaline kood.

    11. Süsteem kontrollib koodi korrektsust.

        2. Kui sisestatud kood on vale, kuvatakse süsteemi poolt teade, et sisestatud kood on vale ja kasutajat ei registeerita.

    12. Järgmisel vormil palutakse sisestada eesnimi, perekonnanimi ja password. Check box võiks olla selleks (by default täidetud), et kasutaja soovib saada infot ridline’i tegemiste kohta.

        3. Password peab olema min 6 kohaline.

        4. Passwordi keerukust kontrollitakse. Selleks annab süsteem tagasisidet 4-kohalisel skaalal.

![image alt text](image_0.png)

    13. Järgmisel vormil süsteem küsib kasutajalt tema peamise rolli kohta (Main role (sound engineer, organizer, artist, venue owner, other). Kasutaja saab antud skippida vajadusel.

    14. Järgmisel formil küsitakse kasutaja eesnime ja perenime (vaja, et kasutajat teistele kasutajatele arusaadavalt display’ida).  Kasutaja saab antud skippida vajadusel.

    15. Süsteem registeerib kasutaja. Süsteem logib kasutaja sisse library vaatesse. Süsteem kuvab teate edukast registreerimisest (modal). 

14. Laiendused (API kaudu registeerimine):

    16. Kasutaja valib API kaudu registeerimise.

    17. Süsteem liidestab kasutaja valitud API’ga (OP.1.4)

    18. Kasutaja sisestab API’le oma kasutajanime, parooli

    19. Süsteem ootab positiivset vastet API kaudu regisreerimisel.

        5. Kui volitus on positiivne JA antud kasutaja pole eelnevalt kasutanud registeerimisel teist API’t, siis jätkatakse punktis 13.9.

        6. Kui volitus on negatiivne, kuvatakse teade, et ei suudetud kasutajat tuvastada ja registeerimine ebaõnnestus.

        7. Kui antud kasutaja on registeeritud teise kasutaja API’ga, siis kuvatakse teade, et kasutaja on juba registeeritud. 

            1. Kasutaja logitakse tema olemasolevasse kontosse library vaatesse.

15. Märkused:

    20.  kastutaja saab alati protsessi pooleli jätta. Selleks igas vaates cancel võimalus.

    21. Kasutaja jääb sisse logituks pärast rakendust väljumist (nt. brauseri akna sulgemisel). Teatud aja pärast rakendatakse automaatne väljalogimine (kasutusjuht "automatic logout")

16. Lahtised probleemid/testimiskohad:

    22. Kuidas kõige vähem kasutajat sisestusandmetega koormata?

    23. Kuidas teha registreerimisprotsessi kiiremaks?

    24. Kas on olemas vigade haldus (nt timeout API’dest jne)?

    25. Passwordi keerukuse kontroll

    26. Kuidas küsida kasutajalt tema peamise rolli kohta?

    27. Kuidas vältida topeltkontosid, kui kasutaja registeerib mitmekordselt erinevate apidega (millele lisaks võib tal olla email:pass meetod)?

    28. Kas captcha lisamine oleks vajalik?

    29. Kuidas vältida, et inimene registeerib erinevate apidega mitu korda?

## 2. Märkused regamise kohta, mida üleval polnud

* Regamine saab alguse ridline.com’st

* Kasutajad, kes määravad enda rolliks muu kui venue (pt. 13.9), viiakse staatilisele lehele sisuga "Under the progress" vms. Miks? Sellepärast, et kui süsteem saab avatuks venudele ja nad saavad hakata sisestama oma andmeid, siis teistel kasutajatüüpidel ei ole 100% töötavaid funktsionaalsusi. Poolikuid asju vist pole mõtet näidata? Variant on ka, et teised rollid praegu üldse välja jätta ja ainult venue jätta.

* Venue kasutajad suunatakse "venue" vaatesse pärast edukat regamist (vt. allpool edasi).

## 3. Venue vaate koostamine

Niiöelda basic template minu nägemuse järgi. Loodan, et pole liiga kosmos.

![image alt text](image_1.png)![image alt text](image_2.png)![image alt text](image_3.png)

![image alt text](image_4.png)

![image alt text](image_5.png)

* Mobile-friendly: kuidas mobiilis tabel ja disain olema hakkab?

* Nimetused (tabelinimed, sektsiooninimed, item’ite nimed) pole siin lõplikud.

* Kui on muudatused salvestamata, siis küsitakse väljalogimisel "kas soovite salvestada?"

* Muudatused salvestatakse automaatselt nagu Google Drive’s (üleval näha ntx "all changes saved")

* Background photo panna kogu body’ile?

* Scrollimine võiks toimuda pidevalt üle lehtede. Continous scrolling. St. profile data’lt läheb üle sujuvalt teistesse vaadetesse jne.

* Praegusel hetkel kasutajad oma rolli muuta ei saaks profiili vaates - venue’d jäävad venue’ks nt.

* Väljade jms elementide paiknemine mockupidel. Kuidas paremini paigutada?Tabeli reeglid:

* Tabiga saab liikuda väljalt väljale juhul, kui üks väli on sisestuseks aktiveeritud. Vasakult paremale. Ülevalt alla. Nagu excelis.

* Saab tekitada kategooriaid juurde. (nupp selle jaoks). Uus kategooria lisatakse kõige alla.

* On olemas teatud standardveerud helitehnika, valgustehnika tabelis (kogus - int, kasutatav - boolean, rendiks - boolean, rendi hind - string, seisund - string) koos vastavate andmetüüpidega.

* Saab tekitada ridu juurde. (nupp selle jaoks). Uus rida lisatakse selekteeritud välja alla. Kui ei ole midagi selekteeritud, siis lisatakse tabeli lõppu.

* Andmed salvestatakse automaatselt.

* On olemas undo võimalus (nupp selle jaoks?)

* Juhul, kui ollakse tabeli lõpus, siis tab tekitab uue rea.

* Saab taastada tabelites algse seisu (nii nagu oli ennem andmete sisestamist). Sel juhul küsitakse kindlasti kinnitust koos hoiatusega, et andmed lähevad kaotsi.

* Tabelis olevaid ridu saab liigutada üles-alla üksida ja koos teiste ridadega. -  Juhul kui liigutan ühte eset, siis teised peavad sellega koos kaasa liikuma (näiteks saan valida kolm eset ja neid korraga liigutada). NB! Kui koos ridasid liigutada, siis saab liigutada ainult  järjestikku olevaid ridasid. 

* Ükski veerg pole kohustuslik.

* Tabelis olevat infot saab selekteerida, kopeerida, kustutada, cuttida (keyboard shortcutid, kontextmenüü)

## 3. Kui kasutajad peaksid uuesti sisselogima

* Venue rolliga kasutajad satuvad venue vaatesse (vt. üleval 2. punkt).

* Teiste rollidega kasutajad satuvad staatilisele lehele a la "We are working to enable sound engineers use our platform" vms juhul, kui teiste rollidega kasutajad saavad üldse praegu süsteemis regada.

## 4. Mida veel:

* Praegu ei ole seda keissi, kui kasutaja peaks oma parooli ära unustama

