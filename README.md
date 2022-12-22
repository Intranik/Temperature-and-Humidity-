# Temp_And_humid
# Temperatur och Luftfuktighetssensor
## Inledning 
En temperatur- och luftfuktighetssensor är en enhet som mäter och registrerar temperaturen och luftfuktigheten i en given miljö. Dessa sensorer kan användas i en mängd olika applikationer, såsom övervakning av temperatur och luftfuktighet i ett växthus, ett förråd eller ett kontorsutrymme.
För att använda en temperatur- och fuktighetssensor med en Arduino, måste du ansluta sensorn till Arduino-kortet med hjälp av kablar. Det finns många olika typer av temperatur- och luftfuktighetssensorer tillgängliga, för att kommunicera med arduio.
## Komponenter
* Arduino Uno.
* DHT11 Sensor (Temperatur och luftfuktighetssensor).
* Breadboard.
* Kablar.
* LCD skärm.
* Resistorer 10K
* MongoDB Database
## Beskrivning
När sensorn är ansluten till Arduino kan du använda Arduinos programmeringsspråk (vanligtvis C++ eller en variant av det) för att läsa temperatur- och luftfuktighetsvärdena från sensorn. Du kan sedan använda denna data för en mängd olika ändamål, som att visa den på en LCD-skärm, logga den till en fil eller skicka den till en fjärrserver för lagring och analys.
För att lagra temperatur- och fuktighetsdata i en MongoDB-databas måste du installera MongoDB-databasprogramvaran på en dator eller server och ställa in en databasanslutning från Arduino till MongoDB-servern. När anslutningen är upprättad kan du använda Arduinos programmeringsspråk för att infoga temperatur- och fuktighetsdata i databasen som dokument.

Denna kod kommer att ansluta till MongoDB-servern på IP-adressen 192.168.1.10 på port 27017, och sedan infoga ett nytt dokument i sensor_data-insamlingen för varje temperatur- och fuktighetsmätning som tas av sensorn. Dokumentet kommer att innehålla temperatur- och luftfuktighetsvärdena samt en tidsstämpel som anger när mätningen gjordes.

Du kan sedan använda verktyg som MongoDB Compass eller MongoDB-skalet för att fråga och analysera data som lagras i databasen.
