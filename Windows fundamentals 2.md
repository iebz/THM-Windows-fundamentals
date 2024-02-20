# Windows fundamentals 2

## System configuration


L' utilitaire de configuration système MSConfig ( ) est destiné au dépannage avancé et son objectif principal est d'aider à diagnostiquer les problèmes de démarrage. 

Référencez le document suivant  ici  pour plus d'informations sur l'utilitaire de configuration système. 

Il existe plusieurs méthodes pour lancer la configuration du système. Une méthode consiste à utiliser le menu Démarrer.

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/9c3cbd2b-3f04-4126-953d-1ba1e86bc00b)

Remarque : Vous avez besoin des droits d'administrateur local pour ouvrir cet utilitaire. 

L'utilitaire comporte cinq onglets en haut. Vous trouverez ci-dessous les noms de chaque onglet. Nous couvrirons brièvement chaque onglet de cette tâche.

1-General

2-Boot

3-Services

4-Startup

5-Tools

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/ec846e24-1577-4e27-b7a0-f5551c853163)

Dans l' onglet Général , nous pouvons sélectionner les appareils et services que Windows doit charger au démarrage. Les options sont : Normal , Diagnostic ou Sélectif . 

Dans l' onglet Boot , nous pouvons définir diverses options de démarrage pour le système d'exploitation.

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/4c17ad3d-ba97-4e86-a98f-9acb4a5bb307)

L' onglet Services répertorie tous les services configurés pour le système, quel que soit leur état (en cours d'exécution ou arrêté). Un service est un type particulier d’application qui s’exécute en arrière-plan. 

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/b8026ef2-3c45-4f6b-9cee-35294c18afe3)

Dans l' onglet Démarrage , vous ne verrez rien d'intéressant dans la VM attachée. Vous trouverez ci-dessous une capture d'écran de l'onglet Démarrage de MSConfig depuis ma machine locale. 

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/29fd3820-66f2-4738-8f16-8761e6de73a0)


Comme vous pouvez le constater, Microsoft conseille d'utiliser le Gestionnaire des tâches ( taskmgr)  pour gérer (activer/désactiver) les éléments de démarrage. L'utilitaire de configuration système n'est PAS un programme de gestion de démarrage. 

Remarque : Si vous ouvrez le Gestionnaire des tâches pour la VM attachée , vous remarquerez que le Gestionnaire des tâches n'affiche pas d'onglet Démarrage. 

Il existe une liste de divers utilitaires (outils) dans l'onglet Outils que nous pouvons exécuter pour configurer davantage le système d'exploitation. Il y a une brève description de chaque outil pour donner un aperçu de son utilité. 


![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/04fa1bdb-4d3a-4b7a-93f0-63d7adcf7d00)

Notez la section Commande sélectionnée . Les informations contenues dans cette zone de texte changeront selon l'outil.

Pour exécuter un outil, nous pouvons utiliser la commande pour lancer l'outil via l'invite d'exécution, l'invite de commande ou en cliquant sur le Launch bouton. 

## Change UAC settings

Nous continuons avec les outils disponibles via le panneau de configuration du système .

Le contrôle de compte d'utilisateur ( UAC ) a été traité en détail dans les principes fondamentaux de Windows 1 . 

Les paramètres UAC peuvent être modifiés ou même complètement désactivés (non recommandé).

Vous pouvez déplacer le curseur pour voir comment le paramètre modifiera les paramètres UAC et la position de Microsoft sur le paramètre.

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/68be002a-9fe8-43f6-ad4a-193865811303)

## computer management 


Nous continuons avec les outils disponibles via le  panneau de configuration du système  .

La gestion informatique (compmgmt)  comporte trois sections principales :  Outils système ,  Stockage et  Services et applications .
