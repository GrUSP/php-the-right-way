---
isChild: true
---

## Criptazione delle Password con Bcrypt

Alla fine, la maggior parte delle applicazioni PHP, richiedono l'accesso degli utenti. Nomi utente e password (criptate) sono archiviate nella base di dati e usate successivamente per autenticare gli utenti durante l'accesso.

E' importante _criptare_ adeguatamente le password che sono archiviate nelal pase di dati. Se una password non &egrave; criptata e la base di dati viene attaccata o &egrave; accessibile ad utenti di terze parti non autorizzati, tutte le credenziali degli utenti saranno compromesse.

**Criptare una password con Bcrypt**.  E' molto semplce e (a tutti gli effetti) Bcrypt rende impossibile per qualcuno risalire alla versione iniziale della password, anche se la base di dati viene compromessa.

Ci sono diverse librerie Bcrypt per PHP che possono essere usate.

* [Leggi "How to Safely Store a Password" di Coda Hale][1]
* [Usa Bcrypt con PHPAss][2] (strano nome, lo so)

[Back to Top](#top){.top}

[1]: http://codahale.com/how-to-safely-store-a-password/
[2]: http://www.openwall.com/phpass/

