<h1>Oppgave3</h1>
a)<br>
Jeg har valgt å bruke tre channels i denne oppgaven, dette kun for å litt grundigere ilustrere bruken av dem. 
C1 og C2 lagrer hvert sitt tall fra cmd input, C3 lagrer summen når C1 og C2 har blitt summert. <br>
Bruker plassene i os.Args ([]) for å lese inn tallene som blir skrivet i cmd. konverterer dem til ints.<br>
funksjonA bruker tall fra stdin som argument, og dytter dem inn i hver sin channel. Her kalles og en .wait(wg) for å forsikre om at ikke programmet går videre før funksjonB har summert og dyttet summen i C3, hvor den så setter wg.done. Når tallet er summert i funksjonB, henter funksjonA ut tallet fra C3 og printer det ut. <br>
Det er og en annen waitgroup i funksjonA (wg2) som venter på at tallet blir printet ut. 
<br>
b)<br>
Slik jeg har tolket oppgaven skal addtofile lese to tall fra cmd og legge disse inn i en tekstfil. sumfromfile skal tallene fra samme tekstfilen, og skrive summen inn i tekstfilen. addtofile skal også printe ut summen etter den har blitt summert.
<h5>Så dette er recap av løsningen min:</h5>
addtofile må kjøres først med to tall som parametre eks. addtofile 2 2. sumfromfile leser tallene, summerer dem, og skriver summen i tekstfilen. Nå må addtofile kjøres UTEN parametre, og vil da printe ut summen som nå står i tekstfilen. <br>
Altså: om en skriver addtofile med to tall, vil den skrive tallene i fil, om en skriver addtofile UTEN parametre, vil den printe det som står i tekstfilen. 



