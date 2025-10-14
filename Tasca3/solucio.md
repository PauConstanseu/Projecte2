### Recuperant accés a sistemes

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



