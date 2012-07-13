---
isChild: true
---

## Namespace

Come ho gi&agrave; detto, la comunit&agrave; PHP ha un sacco di sviluppatori che creano un sacco di codice. Ci&ograve; significa che il codice PHP di una libreria potrebbe utilizzare lo stesso nome per una _classe_ di un'altra libreria. Quando entrambe le librerie sono usate nello stesso namespace collidono e causano problemi.

I _Namespaces_ risolvono questo problema. Come descritto nel manuale di riferimento di PHP, i namespaces possono essere paragonati alle directory di un filesystem come i _namespace_ ai file; due file con lo stesso nome possono coesistere in directory separate. Allo stesso modo, due classi PHP con lo stesso nome possono coesistere nei namespace PHP separati. E' cos&igrave; semplice.

E' importante per voi usare i namespace all'interno del vostro codice in modo che possa essere utilizzato da altri sviluppatori, senza timore di collisioni tra librerie.

Un modo raccomandato di usare i namespace è indicato in [PSR-0][psr0], che indica una convenzione standard per creare file, classi e namespace.

* [Approfondisci i Namespaces][namespaces]
* [Approfondisci PSR-0][psr0]

[Back to Top](#top){.top}

[namespaces]: http://php.net/manual/en/language.namespaces.php
[psr0]: https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-0.md
