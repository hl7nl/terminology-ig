# Introductie
Het adequaat gebruik van terminologie in gestructereerde uitwisseling is essentieel. Helaas wordt niet altijd even zorgvuldig aan de standaard gehouden, wat leidt tot vervuiling en verwarring: beiden zeer ongewenst in (medische) informatie. Om de implementatie van terminologie in uitwisseling te standaardiseren  is het voornemen om in deze track een begin te maken aan een implementation guide: een registratie van de best-practise.

## Aanleiding voor deze Implementation Guide
Wat statistieken
- In veel XIS systemen kan je ```display``` aanpassen en wordt dit opgeslagen alsof het de ```display``` van de code is.
- In huidige berichten klopt 70% van de display values niet met het codesystem

# Wat is een FHIR Implementatie Gids
## Voorbeelden en onderdelen
- https://terminology.hl7.org/
- http://hl7.org/fhir/us/core/terminology.html
- https://build.fhir.org/ig/HL7/fhir-ips/terminology.html

# Stellingen
- Alleen code is niet voldoende voor adequate uitwisseling. Bij het uitwisselen dient een bronsysteem altijd de laatste versie van de ```display``` opzoeken in het bronstelsel, of de ```display``` in de versie van het concept dat uitgewisseld wordt. 
- Een stelling t.a.v. een afwijkende ```display``` tussen bericht en bronstelsel moet nog geformuleerd worden
- Internationaal aspect (denk ook aan IPS); in NL wordt vanzelfsprekend vaak de NL ```display``` waarde opgeslagen. Wat is de geadviseerde werkwijze voor uitwisselen? Opties: geen display meesturen, laatste lokale versie meesturen, anders? 
- Patient Friendly terms - correcte display term is: patient friendly (nederlands) > nederlands > engels?

# Discussie, wat is de scope van de implementatiegids
  - Hoe gebruik je terminology onderdeel van FHIR in een client? Hoe roep je wat aan.
  - Omgaan met ```display```
  - Correcte display voor uitwisseling (patient friendly nl / nl / en)
  - ...