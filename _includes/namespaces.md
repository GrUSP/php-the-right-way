# Namespaces

Come ho gi&agrave; detto, la comunit&agrave; PHP ha un sacco di sviluppatori che creano un sacco di codice. Ci&ograve; significa che il codice PHP di una libreria potrebbe utilizzare lo stesso nome per una _classe_ di un'altra libreria. Quando entrambe le librerie sono usate nello stesso namespace collidono e causano problemi.

I _Namespaces_ risolvono questo problema. Come descritto nel manuale di riferimento di PHP, i namespaces possono essere paragonati alle directory di un filesystem come i _namespace_ ai file; due file con lo stesso nome possono coesistere in directory separate. Allo stesso modo, due classi PHP con lo stesso nome possono coesistere nei namespace PHP separati. E' cos&igrave; semplice.

E' importante per voi usare i namespace all'interno del vostro codice in modo che possa essere utilizzato da altri sviluppatori, senza timore di collisioni tra librerie.

* [Leggi come funzionano i Namespaces][1]

[Back to Top](#top){.top}

[1]: http://php.net/manual/en/language.namespaces.php
