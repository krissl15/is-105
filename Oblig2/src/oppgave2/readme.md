
<h1>Oppgave2, filecount</h1>
<h5>Kort forklaring av koden:</h5>
Funksjonen filecount tar en string som parameter, i main funksjonen blir dette os.Args[1], altså det som skrives etter "filecount" i cmd. <br>
Gjør tekstfilen til string, så til []rune. Oppretter deretter et map med rune som key, og antall ganger brukt som value.<br>
Oppretter deretter en struct samme som mappet, og sorterer structet etter values. Valuesene (antall ganger brukt), blir da sortert etter hvor mange ganger runen er anvendt i teksten. <br>
En for løkke som printer ut de fem mest brukte runene. <br>
Se mer dokumentasjon i kodene.
<br> output:
<img src="https://i.imgur.com/PAUFm8H.png" alt="opg2Output">
<br>
(ja, unicode 32 er space): <img src="https://i.imgur.com/afaPBYD.png" alt="asciiTable">


