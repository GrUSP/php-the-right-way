# Guida alla formattazione del codice

La comunità PHP è ampia ed eterogenea, composta da innumerevoli librerie, framework e componenti. E' normale per gli sviluppatori PHP di scegliere alcuni di questi ed utilizzarli in un unico progetto. E' però importante, per il codice PHP aderire (il più vicino possibile) ad uno stile di codice comune per rendere più facile agli sviluppatori di combinare varie librerie per i loro progetti.

Il [Framework Interop Group][fig] (conosciuto anche come 'PHP Standards Group') ha proposto ed approvato una serie di guide alla formattazione del testo e scrittura del codice, conosciute come [PSR-0][psr0], [PSR-1][psr1] e [PSR-2][psr2]. Non lasciatevi però confondere da queste strane sigle, queste raccomandazione sono semplicemente un insieme condiviso di regole che alcuni progetti come Drupal, Zend, CakePHP, phpBB, AWS SDK, FuelPHP, Lithium, etc hanno iniziato ad utilizzare. Potete usarle nel vostro progetto, o continuare ad usare il vostro personale stile.

Idealmente dovresti scrivere il codice PHP affinchè aderisca a uno più di questi standard in modo tale che altri sviluppatori possano facilmente leggere e lavorare con il tuo codice. Gli standard sono dipendenti da quelli precedenti, ad esempio usando PSR-1 il codice dovrà essere conforme a PSR-0, ma potrebbe non esserlo con PSR-2.

* [Informati su PSR-0][psr0]
* [Informati su PSR-1][psr1]
* [Informati su PSR-2][psr2]

[Back to Top](#top){.top}

[fig]: http://www.php-fig.org/
[psr0]: https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-0.md
[psr1]: https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-1-basic-coding-standard.md
[psr2]: https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-2-coding-style-guide.md
