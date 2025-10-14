# Recuperant accés a sistemes

---

## 1. Introducció

Treballarem sobre una còpia del disc d’un portàtil amb Zorin OS dins d’una màquina virtual per recuperar l’accés d’un usuari que ha oblidat la contrasenya, sense tocar l’equip original. Primer arrencarem la VM amb el disc clonat, obtindrem accés d’administrador, identificarem l’usuari i li assignarem una nova contrasenya, comprovant que pot iniciar sessió. Després investigarem i aplicarem mesures per reforçar l’arrencada (protecció del GRUB amb contrasenya i recomanacions addicionals com xifrat i contrasenya de firmware) per evitar que es repeteixi la mateixa recuperació. Finalment documentarem el procediment amb captures i fonts consultades i lliurarem la VM i un informe resumit amb els passos i recomanacions.

---

## 2. Index

1. Introducció
2. Index
3. Guia

3.1 Vulnereu l’accés al GRUB del Linux.

3.2 Identifiqueu l’usuari del sistema.

3.3 Modifiqueu la contrasenya de l’usuari i verifiqueu que ara ja té accés.

3.4 Investigueu com es pot fortificar l’accés al GRUB. És molt important que indiquis les fonts d’informació que usis.

3.5 Configura la màquina virtual per tal de fortificar l’accés al GRUB

--

## 3. Guia

Primer de tot crearem una màquina virtual amb el disc ja creat anteriorment.
![CreantMV](/Tasca3/img/captura1.png)


### Vulnereu l’accés al GRUB del Linux.

Un cop creada, al entrar li donarem ràpidament al shift+qualsevol tecla del teclat i en sortirà un menú, escollirem la segona opció i al següent menu també escollirem la segona opció.
Llavors ens sortirà aquest menú:

![MenúRoot](/Tasca3/img/captura2.png)

I li donarem a root.


Ara ja estarem dins del GRUB.

![Dins del GRUB](/Tasca3/img/captura3.png)

Ara per canviar la contrasenya del compte és molt fàcil i haurem de seguir aquests senzills passos:

### Identifiqueu l’usuari del sistema.

Primer de tot posarem **ls /home** i així en sortirà el nom d’usuari, en aquest cas es diu miquel.

![Comanda ls /home](/Tasca3/img/captura4.png)

### Modifiqueu la contrasenya de l’usuari i verifiqueu que ara ja té accés.

Seguidament posarem la comanda **passwd + el nom d’usuari (en el meu cas miquel)**, i li posarem la nova contrasenya.

![Comanda per canviar contrasenya](/Tasca3/img/captura5.png)

Li he posat hola1234 de contrasenya.

### Investigueu com es pot fortificar l’accés al GRUB. És molt important que indiquis les fonts d’informació que usis.

El que farem per fortificar l’accés al GRUB serà el següent:

Escriurem la comanda **sudo grub-mkpasswd-pbkdf2** i el que ens surti a partir de grub.pbkdf2.sha512… ho copiarem tot.

Un cop copiat entrarem al arxiu **sudo nano /etc/grub.d/40_custom** i l’editarem de la següent manera:

![Editar arxiu](/Tasca3/img/captura6.png)

Afegirem les dues línies i enganxarem el que haviem copiat abans.

Finalment aplicarem els canvis amb la comanda **sudo grub-mkconfig -o /boot/grub/grub.cfg**.

### Configura la màquina virtual per tal de fortificar l’accés al GRUB

Per fortificar l’accés desde VirtualBox anirem als paràmetres de la nostra màquina virtual, anirem a sistema i on posa ordre d’arrencada deixarem només la del disc dur activat.

![Captura VB](/Tasca3/img/captura7.png)

Seguidament anirem on tenim la carpeta amb el disc virtual, farem clic dret a sobre el disc, li donem a propietats i posarem només lectura, així evitem manipulacions del disc.

![Captura nomes lectura](/Tasca3/img/captura8.png)



**I això seria tot**

---

[Tornar a la pàgina del projecte](../)
