## HL7 Netherlands Terminology FHIR Implementation Guide

Haal de valuesets uit de Nictiz-STU3-Zib2017 repo:
> git clone https://github.com/Nictiz/Nictiz-STU3-Zib2017.git
> cp Nictiz-STU3-Zib2017/Profiles\ -\ ZIB\ 2017/Valuesets/* input/resources/
> cp Nictiz-STU3-Zib2017/Profiles\ -\ ZIB\ 2017/conceptmap-* input/resources/

Genereer de IG:
> java -jar publisher.jar -ig ig.ini
