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

## System information

Nous continuons avec les outils disponibles via le  panneau de configuration du système  .

Qu'est-ce que l' outil Informations système ( msinfo32) ?

Selon Microsoft, " Windows inclut un outil appelé Informations système Microsoft (Msinfo32.exe). Cet outil rassemble des informations sur votre ordinateur et affiche une vue complète de votre matériel, des composants système et de l'environnement logiciel, que vous pouvez utiliser pour diagnostiquer les problèmes informatiques. "

Les informations du résumé du système sont divisées en trois sections :

-Ressources matérielles

-Composants

-Environnement logiciel

Le résumé du système affichera les spécifications techniques générales de l'ordinateur, telles que la marque et le modèle du processeur.

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/41a13f34-1a7e-4fd3-819f-6ff6342cd6c2)

Les informations affichées dans Ressources matérielles ne sont pas destinées à l'utilisateur d'ordinateur moyen. Si vous souhaitez en savoir plus sur cette section, reportez-vous à la page officielle de Microsoft .

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/1290913f-3eee-43c2-a1b1-01c55c216836)

Sous Composants , vous pouvez voir des informations spécifiques sur les périphériques matériels installés sur l'ordinateur. Certaines sections n'affichent aucune information, mais d'autres le font, comme Display et Input .

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/78545ed5-b05c-43bb-aad1-45682280dc76)

Dans la section Environnement logiciel , vous pouvez voir des informations sur les logiciels intégrés au système d'exploitation et les logiciels que vous avez installés. D'autres détails sont également visibles dans cette section, tels que les variables d'environnement et les connexions réseau . 

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/54405d87-79a6-4000-b6b6-75a5e4e02a3a)

Rappel de la salle Windows Fundamentals 1  (tâche du dossier Windows\System32) où  les variables d'environnement  ont été brièvement abordées. 

Selon Microsoft , « Les variables d'environnement stockent des informations sur l'environnement du système d'exploitation. Ces informations incluent des détails tels que le chemin du système d'exploitation, le nombre de processeurs utilisés par le système d'exploitation et l'emplacement des dossiers temporaires.

Les variables d'environnement stockent les données utilisées par le système d'exploitation et d'autres programmes. Par exemple, la variable d'environnement WINDIR contient l'emplacement du répertoire d'installation de Windows. Les programmes peuvent interroger la valeur de cette variable pour déterminer où se trouvent les fichiers du système d'exploitation Windows ".

Cliquez sur Environment Variablespour voir les valeurs attribuées à la machine virtuelle.

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/b71a68a3-37a8-4acb-9aac-7616270020d9)

Une autre méthode pour afficher les variables d'environnement est 

Control Panel > System and Security > System > Advanced system settings > Environment Variables

OR 

Settings > System > About > system info > Advanced system settings > Environment Variables .

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/a7f4c343-2b40-4976-9f16-482c2cc766fa)

Le détour est terminé. Redirigeons notre attention msinfo32et reprenons là où nous nous sommes arrêtés.

Tout en bas de cet utilitaire, il y a une barre de recherche. S'il vous plaît, essayez-le. Sélectionnez Composants et recherchez IP address.

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/1bf4bd42-2f76-4672-bf64-f465f6191385)

## Ressource monitor

Nous continuons avec les outils disponibles via le  panneau de configuration du système  .

Qu'est-ce que le Moniteur de ressources ( resmon) ?

Selon Microsoft, " Resource Monitor affiche des informations par processus et globales sur l'utilisation du processeur , de la mémoire, du disque et du réseau, en plus de fournir des détails sur les processus qui utilisent des descripteurs et des modules de fichiers individuels. Le filtrage avancé permet aux utilisateurs d'isoler les données liées à un ou plusieurs processus (applications ou services), démarrer, arrêter, mettre en pause et reprendre les services et fermer les applications qui ne répondent pas à partir de l'interface utilisateur. Il comprend également une fonctionnalité d'analyse de processus qui peut aider à identifier les processus bloqués et les conflits de verrouillage de fichiers afin que l'utilisateur peut tenter de résoudre le conflit au lieu de fermer une application et potentiellement de perdre des données. "

Comme certains des autres outils mentionnés dans cette salle, cet utilitaire s'adresse principalement aux utilisateurs avancés qui doivent effectuer un dépannage avancé sur le système informatique.

Dans l'onglet Présentation, Resmon comporte quatre sections :

-CPU

-Disque

-Réseau

-Mémoire

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/3238a65c-7314-4a64-9324-8864a0cc6882)

Les quatre mêmes sections ont des onglets correspondants en haut. Voir ci-dessous.

CPU

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/33a62993-8b42-43b3-8753-454980ef0cc8)

Mémoire

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/9190061f-d329-48ce-b2c6-9be1a354e7c4)

Disque

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/c4ab0fa2-09a0-4683-83c0-c70b28eacdbe)


Réseau

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/c7cabe01-befa-45e2-b300-8f7f955989f3)


Bien qu'il ne soit capturé dans aucune des images ci-dessus, Resource Monitor comporte un volet à l'extrême droite. Ce volet affiche une vue graphique en temps réel pour chaque section. 

Remarque : Les informations affichées dans Resource Monitor seront différentes pour vous par rapport aux images ci-dessus.

## CMD

Nous continuons avec les outils disponibles via le  panneau de configuration du système  .

L'invite de commande ( cmd) peut sembler intimidante au début, mais ce n'est vraiment pas si grave une fois que vous avez compris comment interagir avec elle. 

Dans les premiers systèmes d'exploitation, la ligne de commande était le seul moyen d'interagir avec le système d'exploitation.

Lorsque l' interface graphique (interface utilisateur graphique) a été introduite, elle permettait aux utilisateurs d'effectuer des tâches complexes en quelques clics sur un bouton au lieu de saisir des commandes dans l'invite de commande. 

Même si l' interface graphique constitue le principal moyen d'interagir avec le système d'exploitation, un utilisateur d'ordinateur peut toujours interagir via l'invite de commande. 

Dans cette tâche, nous ne couvrirons que quelques commandes qu'un utilisateur d'ordinateur peut exécuter dans l'invite de commande pour obtenir des informations sur le système informatique.

Commençons par quelques commandes simples, telles que hostnameet whoami.

La commande hostname affichera le nom de l'ordinateur.

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/8f01ef23-258d-41e1-a1ba-705f9f96c8e5)

La commande whoami affichera le nom de l'utilisateur connecté.

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/c40660d9-f84a-4e29-8325-1b2b7d840964)

Examinons ensuite quelques commandes utiles lors du dépannage.

Une commande souvent utilisée est ipconfig. Cette commande affichera les paramètres d'adresse réseau de l'ordinateur.

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/7bb39fcc-6ff9-4e64-8b76-6be82c13c14e)

Chaque commande aura un manuel d'aide pour expliquer la syntaxe attendue pour exécuter correctement la commande, ainsi que tous les paramètres supplémentaires pouvant être ajoutés à la commande pour étendre son exécution.

Une commande pour récupérer le manuel d'aide d'une commande est  /?.

Par exemple, pour consulter le manuel d'aide de ipconfig , vous pouvez utiliser la commande suivante :ipconfig /?

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/6f1ffc59-12ec-422e-8e59-c223664b650d)

Remarque : Pour effacer l'écran d'invite de commande, la commande est cls. 

La commande suivante est netstat. Selon le manuel d'aide, cette commande affichera les statistiques du protocole et les connexions réseau TCP/IP actuelles. 

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/7ae9fe4a-2f51-4403-9563-2122a40dc004)

Dans l'image ci-dessus, la ligne dans la case rouge nous montre un exemple de syntaxe pour la commande. 

La structure nous indique que la commande netstat peut être exécutée seule ou avec des paramètres tels que -a,  -b,  -e, etc. 

Lorsque l'un des paramètres est ajouté à la commande racine, netstat dans ce cas, la sortie change. Jouez avec quelques-uns pour voir par vous-même. 

La netcommande est principalement utilisée pour gérer les ressources réseau. Cette commande prend en charge les sous-commandes.

Si vous tapez net sans sous-commande, la sortie affichera la syntaxe de la commande racine montrant quelques-unes des sous-commandes que vous pouvez utiliser.

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/b8abdf71-cb37-4c89-ba94-cfdbff005e04)

Pour la commande net, afficher le manuel d’aide /?ne fonctionnera pas. Dans ce cas, vous devez utiliser une syntaxe différente, à savoir net help.

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/02761d13-7e96-4a52-b08d-671a8f39d441)

Donc, si vous souhaitez voir les informations d'aide pour net user , la commande est net help user. 

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/36a2639a-8c63-4ffb-9f06-689f13bfc8b6)

Vous pouvez utiliser la même commande pour afficher les informations d'aide pour d'autres sous-commandes net utiles , telles que localgroup , use , share et session . 

Reportez-vous au lien suivant pour voir une liste complète des commandes que vous pouvez exécuter dans l'invite de commande ici . 

## Registry Editor


Nous continuons avec les outils disponibles via le  panneau de configuration du système  .

Le registre Windows (par Microsoft) est une base de données hiérarchique centrale utilisée pour stocker les informations nécessaires à la configuration du système pour un ou plusieurs utilisateurs, applications et périphériques matériels.

Le registre contient des informations auxquelles Windows fait continuellement référence pendant le fonctionnement, telles que :

-Profils pour chaque utilisateur

-Applications installées sur l'ordinateur et types de documents que chacune peut créer

-Paramètres de la feuille de propriétés pour les dossiers et les icônes d'application

-Quel matériel existe sur le système

-Les ports qui sont utilisés.

Attention : Le registre est destiné aux utilisateurs d'ordinateurs avancés. Apporter des modifications au registre peut affecter le fonctionnement normal de l'ordinateur. 

Il existe différentes manières d'afficher/modifier le registre. Une solution consiste à utiliser l' éditeur de registre ( regedit).

![image](https://github.com/iebz/THM-Windows-fundamentals/assets/158310804/a51e1882-2c07-4e33-9fb9-2e2db3f88390)

Reportez-vous à la documentation Microsoft suivante ici pour en savoir plus sur le registre Windows. 
