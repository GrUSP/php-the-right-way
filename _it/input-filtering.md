# Filtrare l'input

Nel vostro codice PHP non dovete mai e poi mai ( _ma proprio mai_ ) dar fiducia all'input proveniente dall'esterno. E' un attaggiamento che porta in luoghi oscuri e pericolosi. Invece, &egrave; opportuno filtrare sempre l'input esterno prima di usarlo.

PHP fornisce le funzioni di `filter_var` e `filter_input` per aiutarti a farlo. Queste due funzioni ripuliscono il testo, ne verificano il formato (ie. che sia un'email valida) e fanno l'escape dei caratteri.

Ad esempio, se accetti codice da una form HTML, dovrai usare la funzione di `filter_input` prima di usarla come input per un database o per inserirne il contenuto nell'HTML restituito.

* [Impara ad usare `filter_var`][1]
* [Impara ad usare `filter_input`][2]

[Back to Top](#top){.top}

[1]: http://php.net/manual/en/function.filter-var.php
[2]: http://www.php.net/manual/en/function.filter-input.php
