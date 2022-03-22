# Introductie
Het adequaat gebruik van terminologie in gestructereerde uitwisseling is essentieel. Helaas wordt niet altijd even zorgvuldig aan de standaard gehouden, wat leidt tot vervuiling en verwarring: beiden zeer ongewenst in (medische) informatie. Om de implementatie van terminologie in uitwisseling te standaardiseren  is het voornemen om in deze track een begin te maken aan een implementation guide: een registratie van de best-practise.

## Aanleiding voor deze Implementation Guide
Wat statistieken
- In veel XIS systemen kan je ```display``` aanpassen en wordt dit opgeslagen alsof het de ```display``` van de code is.
- In huidige berichten klopt 70% van de display values niet met het codesystem

# Wat is een FHIR Implementatie Gids
## Bronnen
- Terminologieserver HL7 int: https://terminology.hl7.org/
- Voorbeeld US core terminology: http://hl7.org/fhir/us/core/terminology.html
- Voorbeeld IG: https://build.fhir.org/ig/HL7/fhir-ips/terminology.html
- Confluence terminologie HL7 NL: https://confluence.hl7.org/display/HNETH/Terminology

# Standpunten
- Alleen een ```concept.code``` is niet voldoende voor adequate uitwisseling. Bij het uitwisselen dient een bronsysteem altijd de laatste versie van de ```display``` uit het bronstelsel mee te sturen, of de ```display``` in de versie van het concept dat uitgewisseld wordt wanneer een specifieke versie bedoeld wordt. Ook al is de ```code``` in principe voldoende voor gestructureerde uitwisseling, adviseert de werkgroep het meesturen van een ```display``` voor het geval de ontvangende partij het stelsel niet in bezit heeft. 
- De werkgroep is van mening dat een ```display``` in uitwisseling niet af mag wijken van de ```display``` in het bronstelsel.
- Een eventuele context of aanvullende details kunnen in de text property van een ```codeableConcept``` opgeslagen worden.
- In internationale uitwisseling kan eventueel een Engelse of anders toepasselijke ```display``` worden meegestuurd
- Patient Friendly terms - in het algemeen dient de meest specifieke ```display``` gebruikt te worden. In het geval van uitwisseling naar bijvoorbeeld een PGO kan op basis van context een patiëntvriendelijke term getoond worden. Correcte ```display``` term zou in dit geval kunnen zijn: patient friendly (Nederlands) > Nederlands > Engels.

# Discussie, wat is de scope van de implementatiegids
  - Hoe gebruik je terminology onderdeel van FHIR in een client? Hoe roep je wat aan. Queries?
  - HL7 $validator connectie met NTS
    - Nu door authenticatieproblemen niet nodig
    - @Roel Barelds neemt contact op met Nictiz
  - Crowdsourced vertalingen
    - Voorstel van de groep om een systeem voor crowdsourcen van missende vertalingen voor terminologie op te zetten.
    - Feikje Hielkema, Nictis terminologiecentrum:


      Hoi Roel,

      Voor onvertaalde SNOMED-codes wil ik jullie toch met klem aanraden om een vertaling bij ons aan te vragen. Als het volume niet al te hoog is (beperkt tot hooguit een paar honderd), pakken we dit direct op en heb je een officiële vertaling bij de volgende SNOMED-editie. Voor patiëntvriendelijke vertalingen voor SNOMED kun je het beste overleggen met mijn collega Natasha Krul.
      Wat zijn de andere stelsels waar vertalingen ontbreken? LOINC neem ik aan, maar wat nog meer? Voor LOINC en UCUM sluit ik graag aan. Voor andere stelsels hebben we wellicht weer andere collega’s nodig 😊

      Groeten,

      Feikje