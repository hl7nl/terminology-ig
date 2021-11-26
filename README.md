## HL7 Netherlands Terminology FHIR Implementation Guide

Inhoudsopgave onderwerpen
* Inleiding (zie ook https://confluence.hl7.org/display/HNETH/Terminology+Kick-off+%28Hands-on%29+Implementatie+Gids+NL+16e+HL7-WGM)
    - In veel XIS systemen kan je displayName aanpassen
    - Dit leidt tot de situatie waar in huidige berichten 70% van de display values niet klopt met het codesystem: of dit een wenselijke situatie is, is onderwerp van discussie
    - Bovenstaande is wat de werkgroep betreft aanleiding tot het schrijven van een landelijke richtlijn voor het gebruik van terminologie in zorgsystemen (incl de context van uitwisseling)
* Samenwerking
** HL7 NL en Nictiz NTS
    - De Nationale Terminologieserver van Nictiz biedt de mogelijkheid om terminologie te valideren tegen de meest recente versie in de Nederlandse taal. Voor deze server ook werkt met de HL7 validator zijn er een aantal stappen nodig

** Relatie met HL7 International HTA/Vocab/TSMG
* Community vertalingen
** Mogelijke tool https://crowdin.com 
    - @Hidde maakt voorbeeld
    - Validatie door gecertificeerd terminologen - inzet Nictiz?
    - Overname in release van bv SNOMED?

* Waar zijn de codesystemen in beheer? 
* Bronsystemen
** Voorbeeld Rol van de NTS en hoe de NTS te gebruiken 
* Use-guide / implementatie
** Eisen aan gebruik en vulling, e.g. displayName vs text
** Howto: Opzoeken patient vriendelijke termen, zowel functioneel als technisch (met FHIR API)
* Eisen aan coderingen
* Alle in de NL gebruikte codesystemen en valuesets en mappings (vanuit FHIR Profiles en zibs) of een verwijzing
* References (Verzamelen eisen in huidige informatiestandaarden, MedMij, Nictiz)
** e.g. https://informatiestandaarden.nictiz.nl/wiki/MedMij:V2020.01/FHIR_IG#Use_of_coded_concepts 
** https://informatiestandaarden.nictiz.nl/wiki/FHIR:V1.0_FHIR_Profiling_Guidelines_STU3 
** https://informatiestandaarden.nictiz.nl/wiki/FHIR:V1.0_FHIR_Profiling_Guidelines_R4 
** https://www.nictiz.nl/standaardisatie/terminologiecentrum/nationale-terminologieserver/ 
** https://informatiestandaarden.nictiz.nl/wiki/MedMij:V2020.01/FHIR_IG 
** https://www.nictiz.nl/wp-content/uploads/Leidraad-Terminologie-Nictiz.pdf
