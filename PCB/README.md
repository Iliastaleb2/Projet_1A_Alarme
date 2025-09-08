# Description

Plus précisément, lorsque le faisceau LASER est interrompu, une alarme à deux tons ou à progression sinusoïdale (ajustable via un cavalier) est déclenchée.
Pour arrêter l’alarme, différents codes doivent être saisis, avec un « supercode » permettant malgré tout de stopper l’alarme en cas d’erreur de saisie des codes.

Avec mon partenaire, notre rôle était de gérer la sortie, c’est-à-dire le signal sonore et la variation de fréquence à partir d’un signal carré transmis par le microcontrôleur STM32L476RG entre 0 et 3,3 V.

Pour cela, nous avons principalement utilisé :

Un VCO (XR2206 pour générer le signal et basculer entre bi-ton et progressif)

Des transistors (NPN 2N1711 et PNP 2N2905 pour amplifier le signal)

Un convertisseur IA1215S DC-DC (12 V vers 15 V pour alimenter le circuit audio)

Un ampli-op TL082 (pour intégrer et inverser le signal)

Un haut-parleur KSSG1708

## Schématique : 
<img width="1215" height="832" alt="image" src="https://github.com/user-attachments/assets/3ad432f5-4893-4842-aa66-c62201c0f591" />

## Bottom :


<img width="406" height="350" alt="image" src="https://github.com/user-attachments/assets/bc5b6d14-19f6-438b-a74a-e80c789dcee5" />
<img width="960" height="1280" alt="image" src="https://github.com/user-attachments/assets/4e9ed21e-c2e1-413c-a023-2db3975203e7" />

## Top :


<img width="806" height="789" alt="image" src="https://github.com/user-attachments/assets/2089cfa2-dd40-4ea2-a659-ee5d4180a65e" />
<img width="960" height="1280" alt="image" src="https://github.com/user-attachments/assets/a3e77721-d7ae-4026-830f-a82275e229c2" />

