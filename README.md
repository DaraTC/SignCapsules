# Table of contents

1. [Installation de PowerApps for Teams](#installation-de-power-apps-for-teams)
2. [Importation des thématiques](#importer-les-thématiques-dans-la-table-dataverse-for-teams)
3. [Mise en place des fluxs](#mise-en-place-des-fluxs-dimports-et-de-rappels)
4. [Rajout d'administrateurs](#rajouter-un-administrateur)
5. [Changement des autorisations de table dans Dataverse for Teams](#changer-les-autorisations-de-table-dans-dataverse-for-teams)
6. [Partage de l'application pour un cadre restreint](#partager-lapplication-pour-un-cadre-restreint)
7. [Déploiement de l'application via le manifest dans l’AppSource de Teams](#déployer-lapplication-via-le-manifest-dans-lappsource-de-teams)

### Installation de Power Apps for Teams 

- Installez l’application PowerApps for Teams depuis l’App Source 
- Sélectionnez l’équipe dans laquelle vous voulez importer la solution de Signed Capsules.
- Cliquez sur les 3 petits points à côté du nom de l’équipe puis « Open in PowerApps »  
- Dans les solutions de l’environnement Dataverse for Teams, appuyez sur « Import/Importer » 
- Sélectionnez le package puis sur « Next/Suivant » puis « Import/Importer » 
- Vérifiez que le contenu de la solution est complet. 

### Importer les thématiques dans la table Dataverse For Teams 

- Accédez à l'environnement précedemment créé dans PowerApps for Teams
- Cliquez sur "Tables", sélectionnez ensuite sur "Data" puis enfin "Get Data"
- Selectionnez "Excel Workbook" dans "All Categories"
- Selectionez "Upload Files" puis insérez le fichier .xslx joint au package que vous avez précédemment installé
- Rajoutez au besoin votre connexion personnalisée 
- Cliquez sur "Next", sélectionnez la table "Table1" puis cliquez à nouveau sur "Next" jusqu'à arriver au mappage de la table
- Dans « Source column », sélectionnez Thematic pour la destination Name et Sign Language pour la destination Sign Language 
- Cliquez sur "Publier".
- Vérifiez que les thématiques sont désormais présentes dans la table Dataverse, cela peut prendre quelques minutes.


### Mise en place des fluxs d'imports et de rappels 

##### N.B : Avant toute chose, assurez-vous que vous avez rajouté les thématiques dans la table Thematic en passant par les étapes du 2.   
 
- Dans le site SharePoint de l’équipe Teams (que vous avez précedemment utilisé pour l'environnement), créez une bibliothèque de documents pour l’import des vidéos.
- Récupérez le site SharePoint et la bibliothèque utilisée 
- Dans les deux premières actions du flux [Signed Capsules] Flux d’import de données, remplacez les différentes valeurs avec votre Bibliothèque SharePoint, remettez dans « File Identifier » l’objet « Identifier »  
- Activez le flux et testez en insérant une vidéo dans la bibliothèque en respectant le template de nom de vidéo tel que « (LSF/ASL)-Nom Thématique-Nom vidéo.mp4 
 

### Rajouter un administrateur 

- Accédez à la table « Administrator » de la solution de l’application Signed Capsules. 
- Cliquez ensuite sur "Edit Data".
- Dans la fenêtre qui s’ouvre, rajoutez dans une nouvelle colonne l’email de l’utilisateur qui aura les droits d’administration. 
- Si l’utilisateur avait l’application ouverte, demandez-lui de recharger l’application et l’onglet « Administration » devrait apparaître à côté de « Articles »  

### Changer les autorisations de table dans Dataverse for Teams

- Pour modifier les autorisations de tables dans Dataverse For Teams, accédez aux éléments de la solution de votre équipe Teams depuis l’application PowerApps pour Teams. 
- Cliquez sur la table dont vous voulez changer les permissions puis cliquez sur « Manage Permissions »  
- Vous pourrez ensuite depuis cette page modifier les permissions pour chaque type d’utilisateur (Membres, Invités, Security Group)  

### Partager l'application pour un cadre restreint

- Depuis l’application PowerApps for Teams, cliquez sur Build puis naviguez dans l’équipe où se trouve la solution de l’application « Signed Capsules » 
- En haut à droite se trouve un bouton « Share with collègues/Partagez avec des collègues », cliquez dessus.
- Entrez le security group avec lequel vous voulez partagez l’application, cochez l’application Signed Capsules puis cliquez sur « Save » 
- Les utilisateurs trouveront désormais l’application « Signed Capsules » dans l’App Source de Teams 

### Déployer l'application via le manifest dans l'AppSource de Teams
 
- Récupérez le manifest depuis l’application PowerApps for Teams en sélectionnant l’application dans la liste des items de l’environnement puis en cliquant sur “Add to Teams” et enfin sur “Download App” 
- Dans l’App Source de Teams, cliquez sur “Manage your apps”  
- Cliquez sur “Upload an app” puis sur “Submit an app to your org” 
- Un explorateur de fichier s’ouvre, selectionnez le .zip précedemment téléchargé. 
- L’application sera envoyé à l’équipe en charge du déploiement 
