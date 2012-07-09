# Basi di dati e PDO

Spesso il vostro codice PHP dovr&agrave; utilizzare una base di dati per salvare le informazioni. Se usate una base di dati, usate `PDO` per dialogare con essa. PDO &egrave; una libreria di astrazione &mdash; (solitamente) presente all'interno di PHP &mdash; che fornisce un'interfaccia generica per dialogare con differenti basi di dati.

Ancora pi&ugrave; importante, `PDO` vi consente di inserire in modo sicuro dati provenienti dall'esterno (ad esempio ID) nelle vostre query SQL senza dovervi preoccupare di proteggervi da tentativi di attacco tramite SQL injection. Questo &egrave; possibile utilizzando PDOStatements ed i parametri associati.

Assumiamo che lo script PHP riceva un ID numerico che deve essere usato come parametro della query. Questo ID deve essere utilizzato per estrarre un record dalla base di dati. Questo &egrave; il modo `errato` per farlo:

    <?php
    $pdo = new PDO('sqlite:users.db');
    $pdo->query("SELECT name FROM users WHERE id = " . $_GET['id']); // <-- NO!

Questo codice &egrave; orribile. State inserendo un parametro in maniera grezza all'interno della query. In questo modo sarete attaccati in men che non si dica. In alternativa potete procedere ripulendo l'ID in ingresso utilizzando i parametri associati di PDO.
				
    <?php
    $pdo = new PDO('sqlite:users.db');
    $stmt = $pdo->prepare('SELECT name FROM users WHERE id = :id');
    $stmt->bindParam(':id', filter_input(INPUT_GET, 'id', FILTER_SANITIZE_NUMBER_INT), PDO::PARAM_INT);
    $stmt->execute();

Questo &egrave; il modo corretto di scrivere il codice. Utilizza i parametri associati in una dirittiva PDO, controlla i parametri in ingresso prima che vengano inseriti nel database, prevenendo eventuali attacchi di tipo SQL injeection.

* [Informati su PDO][1]

[Back to Top](#top){.top}

[1]: http://www.php.net/manual/en/book.pdo.php
