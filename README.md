Dashboard 2024 <br>
(attention demande beaucoup de ressource materiel pour etre afficher et opérationnel le problème est en cours de résolution)<br>
un tuto pour l'installation est dispo en bas de page<br>
<br>
update:<br>
28/01/2024: nettoyage du code[terminer]<br><br>
31/01/2024: maintenant le background animé de la carte meteo change en foction de l'état du sensor et ajout du background animé sur la carte horloge (les gif ou images peuvent être changer dans background-image: url(l'url de l'image);<br><br>
<b> &#x26A0;<U><br>Attention il faut modifier la ligne 66 avec le nom de votre ville pour que le changement d'images sois pris en compte</U></b>[terminer]<br><br>
01/02/2024: redaction d'un tuto d'installation[terminer]<br><br>
02/02/2024: meilleur optimisation et nettoyage du code , remplacement chip-card par des chip-card-conditionel , ajout d'un fond pour les informations primaires et secondaires pour une meilleur visibilitée sur le background de la carte[terminer]<br><br>
11/02/2024: modification et externalisation de certain morceau de code du dashboard <br><br>
<U><b> &#x26A0;<U><br>Attention le fichier dashboard est a placer a l'aide de file editor ou studio code server /homeassistant/themes/dashboard 2024/dashboard2024.yaml ,il se peut que le dossier themes et dashboard 2024 ne sois pas créé rajouté le et placer le fichier dashboard2024.yaml a l'interieur, et changer le theme en dashboard 2024 pour cela faite modifier tableau cliquer sur le crayon , dans configuration de la vue dans theme mettre dashboard 2024</U></b>[terminer]<br><br>
23/02/2024: remplacement des background info primaires et secondaires par de simple ombres sous le text pour une meilleur adaptabilitée de l'affichage des different devices (tel,tablette,pc,etc...) et en cas de changement de background [terminer]<br><br>
02/03/2024: mise a jour majeure du code, remplacement de l'addon browser_mod par bubble_card (moins gourmand,plus graphique et plus rapide) , modification de certaines fonction,adaptation des conditions de certaines entitées, (toutes les cartes popup se truve dans la dernière carte de la première ligne) l'installation et l'exploitation reste la meme que la version precedente [terminer]<br>
<br><br>
update en cours:<br>
01/01/2024: résolution des problemes de ressources rencontré pour certain apareils (passage du maximum de parametres de cartes en version theme plutot quand carte modifiée) [en cours]<br>
<br>
Le code des cartes est dans le fichier carte dashboard
pour le sensor "il fait nuit" le lien pour la création https://www.sigalou-domotique.fr/je-voudrais-savoir-si-nous-sommes-le-jour-ou-la-nuit<br>
Addons et intégrations nécessaire.<br>
Addon: 
  - lovelace-meteofrance-weather-card ( https://github.com/hacf-fr/lovelace-meteofrance-weather-card )
  - vertical-stack-in-card ( https://github.com/ofekashery/vertical-stack-in-card )
  - tabbed card (uniquement si pronote est utiliser)( https://github.com/kinghat/tabbed-card )
  - mushroom ( https://github.com/piitaya/lovelace-mushroom )
  - card-mod ( https://github.com/thomasloven/lovelace-card-mod )
  - digital-clock ( https://github.com/wassy92x/lovelace-digital-clock )
  - bubble-card ( https://github.com/Clooos/Bubble-Card )

Integrations:
  - <s>browser mod (pour l'affichage des popup) ( https://github.com/thomasloven/hass-browser_mod )</s> n'est plus necessaire
  - meteo france (pour afficher la meteo)
  - alarmo (si utiliser sinon peut etre supprimer)( https://github.com/nielsfaber/alarmo )
  - pronote (si utiliser sinon peut etre supprimer)( https://github.com/delphiki/hass-pronote )<br><br>
  
Les backgrounds des cartes se trouvent lignes:
  - meteo: 68
  - horloge: 87
  - salon: 239
  - salle a manger: 393
  - cuisine: 523
  - couloir: 625
  - salle de bain rdc: 707
  - chambre parentale: 835
  - chambre d'amis: 944
  - chambre rox: 1051
  - palier: 1158
  - salle de bain etage: 1244
  - chambre ethan: 1351
  - chambre nathan: 1500
<br><br>
![screenshot](https://i.ibb.co/RQ3GLKM/dashboard-0.png)
![screebshot2](https://i.ibb.co/pnqCMtz/dashboard-1.png)

Pour installer le dashboard une fois tout les addons et intégration installé il vous suffit de cliquer en haut a droite de votre dashboard , modifier tableau de bord et de créé un nouveau tableau de bord<br><br>
![screenshot](https://github.com/RomainRou/dashboard/blob/main/2.png)
![screenshot](https://github.com/RomainRou/dashboard/blob/main/3.png)
![screenshot](https://github.com/RomainRou/dashboard/blob/main/4.png)<br><br>
Dans configuration de la vue vous mettez se que vous voulez sauf pour la partie type de vue il faut mettre Panneau (1 carte) et vous sauvegarder<br>
![screenshot](https://github.com/RomainRou/dashboard/blob/main/5.png)<br><br>
Vous cliquez sure ajouter une carte en bas a droite , et vous choisissez la carte manuel ensuite vous copier tout le code en lieu et place de type:'' en prenant soin de le supprimer puis vous sauvegarder et c'est terminer, il vous reste plus qu'a reconfiguré vos entitée etc... et de vous amusez a changer se que vous voulez libre a vous les possibilitées sont nombreuses niveau personalisation <br><br>
![screenshot](https://github.com/RomainRou/dashboard/blob/main/6.png)
![screenshot](https://github.com/RomainRou/dashboard/blob/main/7.png)
