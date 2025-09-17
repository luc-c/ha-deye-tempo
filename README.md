# ha-deye-tempo
Dans le cadre d'un abonnement a l'offre tempo d'EDF et d'avoir une installation photovoltaique avec batterie, il peut etre interessant de charger la batterie la nuit si elle n'est pas chargée par les panneaux photovoltaiques le jour. En effet, durant les periodes d'heures creuse, le cout du Kwh est entre 3 et 4 fois moins cher que le jour. Le focntionnement des onduleurs hybrides DEYE tel que le SUN-6K-SG03LP01 est parametré par une table horaire qui definie les flux en fonction de l'etat de charge de la batterie. Dans un usage normal, on fait charger la batterie le jour avec le surplus d'electricité non consommé. Lorsque la production est nulle ou inferieure a la consomation de sa maison, on consomme cette energie sockée ideallement lorsqu'elle est la plus chere.

Plusieurs etapes peuvent etre envisagées:
  1. Lorsque l'information de tarification du jour suivant est donnée on change le mode de fonctionnement pour permettre la charge durant les heures creuses en cas de jour Rouge. Si c'est un jour Bleu ou Blanc on retabli le focntionnement normal a savoir une charge exclusivement solaire.

Sources:
[Solarman integration in Home Assistant](https://github.com/davidrapan/ha-solarman)
[RTE Tempo in Home Assistant] (https://github.com/hekmon/rtetempo)
