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

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/f70db181-b512-4c1b-a529-ea5449788f31)

Outils système

Commençons par le Planificateur de tâches . Selon Microsoft, avec Task Scheduler, nous pouvons créer et gérer des tâches courantes que notre ordinateur exécutera automatiquement aux heures que nous précisons.

Une tâche peut exécuter une application, un script, etc., et les tâches peuvent être configurées pour s'exécuter à tout moment. Une tâche peut s'exécuter à la connexion ou à la déconnexion. Les tâches peuvent également être configurées pour s'exécuter selon un calendrier spécifique, par exemple toutes les cinq minutes.

Pour créer une tâche de base, cliquez sur Create Basic Tasksous Actions (volet de droite).

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/2256b601-1f80-47b3-82c6-7292e157c6d8)

Vient ensuite l’Observateur d’événements .

L'Observateur d'événements nous permet de visualiser les événements qui se sont produits sur l'ordinateur. Ces enregistrements d'événements peuvent être considérés comme une piste d'audit permettant de comprendre l'activité du système informatique. Ces informations sont souvent utilisées pour diagnostiquer les problèmes et enquêter sur les actions exécutées sur le système. 

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/7ba0de6c-6f98-496a-8f9d-83fd0bd374a2)

L'Observateur d'événements comporte trois volets.

1-Le volet de gauche fournit une arborescence hiérarchique des fournisseurs de journaux d'événements. (comme le montre l'image ci-dessus)

2-Le volet du milieu affichera un aperçu général et un résumé des événements spécifiques à un fournisseur sélectionné.

3-Le volet de droite est le volet Actions.

Il existe cinq types d'événements pouvant être enregistrés. Vous trouverez ci-dessous un tableau de  docs.microsoft.com  fournissant une brève description de chacun.

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/f848f778-a65b-46dc-b06c-9efc134f69af)

Les journaux standard sont visibles sous  Journaux Windows . Vous trouverez ci-dessous un tableau de  docs.microsoft.com  fournissant une brève description de chacun.

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/24f52290-3876-4668-9f6c-1ed065f08b9b)


Pour plus d'informations sur l'Observateur d'événements et les journaux d'événements, veuillez vous référer à la salle des journaux d'événements Windows . 

Les dossiers partagés sont l'endroit où vous verrez une liste complète des partages et des dossiers partagés auxquels d'autres peuvent se connecter. 

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/7c5cc01d-2e37-478f-a155-612f649c2ecc)

Dans l'image ci-dessus, sous Partages, se trouvent le partage par défaut de Windows, C$ et les partages d'administration à distance par défaut créés par Windows, tels que ADMIN$. 

Comme pour tout objet Windows, vous pouvez cliquer avec le bouton droit sur un dossier pour afficher ses propriétés, telles que les autorisations (qui peut accéder à la ressource partagée). 

Sous Sessions , vous verrez une liste des utilisateurs actuellement connectés aux partages. Dans cette VM , vous ne verrez personne connecté aux partages.

Tous les dossiers et/ou fichiers auxquels accèdent les utilisateurs connectés seront répertoriés sous Open Files .

La section Utilisateurs et groupes locaux que vous devriez connaître dans Windows Fundamentals 1 car il s'agit de lusrmgr.msc.

Dans Performance , vous verrez un utilitaire appelé Performance Monitor ( perfmon).

Perfmon est utilisé pour afficher les données de performances en temps réel ou à partir d'un fichier journal. Cet utilitaire est utile pour résoudre les problèmes de performances sur un système informatique, qu'il soit local ou distant. 

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/591b1818-c806-47ff-9ef1-55e015faf785)

Le Gestionnaire de périphériques nous permet de visualiser et de configurer le matériel, par exemple en désactivant tout matériel connecté à l'ordinateur.

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/fbc29908-e448-4a75-9e59-26ff81b2e2c2)

Stockage  

Sous Stockage se trouve la sauvegarde et la gestion des disques de Windows Server . Nous examinerons uniquement la gestion des disques dans cette salle.

Remarque : Étant donné que la machine virtuelle est un système d'exploitation Windows Server, il existe des utilitaires disponibles que vous ne verrez généralement pas dans Windows 10.

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/bc1a7982-554a-4d2f-bf1c-002a78f88e3b)

La gestion des disques est un utilitaire système sous Windows qui vous permet d'effectuer des tâches de stockage avancées.  Certaines tâches sont :

-Configurer un nouveau lecteur

-Étendre une partition

-Réduire une partition

-Attribuer ou modifier une lettre de lecteur (ex. E :) 

Services et applications

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/29e2379d-1eba-41fd-9d62-f4f1b1e9bd31)

Rappel de la tâche précédente ; un  service est un type spécial d'application qui s'exécute en arrière-plan. Ici, vous pouvez faire plus que simplement activer et désactiver un service, comme afficher les propriétés du service.

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/d6d7891e-955a-440b-88ae-4a5549e703a2)

WMI Control configure et contrôle le service Windows Management Instrumentation ( WMI ).

Selon Wikipédia, « WMI permet aux langages de script (tels que VBScript ou Windows PowerShell) de gérer les ordinateurs personnels et les serveurs Microsoft Windows, à la fois localement et à distance. Microsoft fournit également une interface de ligne de commande à WMI appelée ligne de commande Windows Management Instrumentation (WMIC). . "

Remarque : L'outil WMIC est obsolète dans Windows 10, version 21H1. Windows PowerShell remplace cet outil pour WMI. 
