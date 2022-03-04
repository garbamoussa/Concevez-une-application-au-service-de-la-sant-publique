# Concevez-une-application-au-service-de-la-sant-publique
Concevez une application au service de la santé publique
L'agence "Santé publique France" a lancé un appel à projets pour trouver des idées innovantes d’applications en lien avec l'alimentation. Vous souhaitez y participer et proposer une idée d’application.

Les données
Extrait de l’appel à projets :
Le jeu de données Open Food Facts est disponible sur le site officiel (ou disponible à ce lien en téléchargement). Les variables sont définies à cette adresse.
Les champs sont séparés en quatre sections :
Les informations générales sur la fiche du produit : nom, date de modification, etc.
Un ensemble de tags : catégorie du produit, localisation, origine, etc.
Les ingrédients composant les produits et leurs additifs éventuels.
Des informations nutritionnelles : quantité en grammes d’un nutriment pour 100 grammes du produit.
Votre mission
Après avoir lu l’appel à projets, voici les différentes étapes que vous avez identifiées :
1) Traiter le jeu de données, en :
Réfléchissant à une idée d’application.
Repérant des variables pertinentes pour les traitements à venir, et nécessaires pour votre idée d’application.
Nettoyant les données en :
mettant en évidence les éventuelles valeurs manquantes, avec au moins 3 méthodes de traitement adaptées aux variables concernées,
identifiant et en quantifiant les éventuelles valeurs aberrantes de chaque variable.
Automatisant ces traitements pour éviter de répéter ces opérations
Le programme doit fonctionner si la base de données est légèrement modifiée (ajout d’entrées, par exemple).
2) Tout au long de l’analyse, produire des visualisations afin de mieux comprendre les données. Effectuer une analyse univariée pour chaque variable intéressante, afin de synthétiser son comportement.
L’appel à projets spécifie que l’analyse doit être simple à comprendre pour un public néophyte. Soyez donc attentif à la lisibilité : taille des textes, choix des couleurs, netteté suffisante, et variez les graphiques (boxplots, histogrammes, diagrammes circulaires, nuages de points…) pour illustrer au mieux votre propos.
3) Confirmer ou infirmer les hypothèses à l’aide d’une analyse multivariée. Effectuer les tests statistiques appropriés pour vérifier la significativité des résultats.
4) Justifier votre idée d’application. Identifier des arguments justifiant la faisabilité (ou non) de l’application à partir des données Open Food Facts.
5) Rédiger un rapport d’exploration et pitcher votre idée durant la soutenance du projet.
 Livrables
Un notebook du nettoyage des données (non cleané, pour comprendre votre démarche). 
Un notebook d’exploration comportant une analyse univariée, multivariée, une réduction dimensionnelle, ainsi que les différentes questions de recherches associées (non cleané, pour comprendre votre démarche).
Une présentation, à utiliser en support pour la soutenance, comprenant :
La présentation de votre idée d’application.
Les opérations de nettoyage effectuées.
La description et l'analyse univariée des différentes variables importantes avec les visualisations associées.
L’analyse multivariée et les résultats statistiques associés, en lien avec votre idée d’application.
3 observations solidement étayées (graphes et/ou tests statistiques à l’appui au besoin) évaluant la pertinence et la faisabilité de votre application.
La synthèse des différentes conclusions sur la faisabilité de votre projet.

GUIDE  MENTOR  

L’intention de ce projet est de permettre à l’étudiant de mettre en œuvre des compétences de Data Analyst : cleaning, préparation des données et analyse exploratoire.
Attention, l’analyse peut prendre beaucoup de temps. Assurez-vous que l’étudiant se fixe en amont un certain nombre d'heures maximum sur ce projet d’exploration, et s’y tient.
Vous sensibiliserez l’étudiant à l’importance de ce projet, qui constitue une étape incontournable de toute démarche de Data Science, en préalable à la mise en œuvre d’algorithmes de Machine Learning. Les prochains projets du parcours intègreront naturellement une étape de nettoyage et d’analyse exploratoire des données, que l’étudiant doit donc parfaitement maîtriser.
Vérifiez tout au long de l’accompagnement que l’étudiant met en œuvre et couvre l’ensemble des critères de compétence détaillés ci-dessous.
Incitez l’étudiant à utiliser différentes librairies pour générer les graphiques, Maplotlib, mais également par exemple Seaborn qui propose de nombreuses fonctionnalités puissantes et faciles à mettre en œuvre.
Assurez-vous que l’étudiant oriente bien son projet en fonction de la problématique de la nutrition, en analysant et exploitant les features qui permettent de proposer une idée d’application.
De nombreuses réponses au projet sont possibles.
Une fois la partie analyse exploratoire/data cleaning validée, elle ne sera pas à évaluer formellement de nouveau dans les projets suivants, même si c’est une activité courante du Data Scientist.
Voici un aperçu des étapes suggérées (mais NB que les étudiants ne sont pas tenus de réaliser les étapes du projet dans cet ordre). Cette section met également en évidence les difficultés potentielles. Veuillez noter :
La vitesse d’avancement du projet pour chaque étape est donnée à titre indicatif mais varie en fonction de chaque élève.
Le livrable fait référence aux résultats attendus par l'étudiant. Les étudiants ne sont pas non plus tenus de remplir ces “sous-livrables” suggérés pour valider le projet ; ils ne seront évalués que sur les livrables finaux.
 
Remarque générale :
 Les milestones sont présentés de manière linéaire, mais dans la pratique certains traitements sont itératifs
 Par exemple, une analyse uni-variée de type describe() ou boxplot sera nécessaire initialement pour analyser et traiter les valeurs aberrantes, puis une fois les données complètement nettoyées pour réaliser l’analyse exploratoire demandée dans le deuxième notebook.
Milestone 1 : Nettoyage – Filtrage des features et produits
Livrable :
Notebook de nettoyage, partie filtrage des features et produits
Niveau d’avancement : 20 %
Problèmes et erreurs courants :
Garder trop de features, qui complexifierait le nettoyage et l’analyse
Se limiter à un nettoyage « technique » (taux de remplissage) sans se poser la question des besoins métiers
Recommandations :
Lister l’ensemble des features du fichier, quantitatives (numériques) ou qualitatives (catégorielles)
Afficher le taux de remplissage des features, pour se rendre compte que la très grande majorité des features est très peu remplie
Commencer à réfléchir à une idée d’application qui exploiterait une partie des données une fois nettoyées. L’objectif du projet est de mettre à disposition un fichier de données nettoyées qui pourrait être utilisé pour cette application. Il ne s’agit pas de réaliser cette application. L’analyse exploratoire à partir des données nettoyées se fera dans l’optique de s’assurer que les données permettraient de réaliser cette application
Combiner 2 approches complémentaires :
Approche technique : faire un choix fort de suppression des features pas suffisamment remplies. Un seuil de taux de remplissage autour de 50% est pertinent, à affiner éventuellement ensuite par itération
Approche métier : à partir de l’idée d’application, ne garder que les features et produits qui seraient vraiment utiles pour réaliser cette application
Par exemple, si l’idée d’application est de proposer des produits similaires mais avec un nutriscore meilleur, il peut être pertinent de se limiter à des produits français (un utilisateur n’ira pas aux US pour aller acheter un meilleur produit)
Ne garder que les features catégorielles vraiment utiles pour catégoriser les produits (par exemple pnns_groups_1 ou pnns_groups_2, voire nova_group selon les besoins)
Globalement ne pas hésiter à supprimer rapidement de nombreuses features, afin de faciliter les traitements et les analyses suivantes, quitte à rajouter après coup quelques features
L’étudiant devrait avoir gardé environ 15 à 20 features après cette étape
Supprimer les produits en double, selon un critère à définir par l’étudiant (code produit par exemple).
Milestone 2 : Nettoyage – valeurs aberrantes
Livrable :
Notebook de nettoyage, partie traitement des valeurs aberrantes
Niveau d’avancement : 40 %
Problèmes et erreurs courants :
Erreur de supprimer les outliers selon la méthode interquartile sur l’ensemble des produits, alors qu’ils ne sont pas homogènes
Erreur de filtrer en ne prenant, pour les features numériques pour 100g, que les produits ayant pour valeur >0g et <100g, ce qui supprimerait en conséquence les produits avec une valeur à NaN
Recommandations :
Dans ce projet il est important de privilégier une approche orientée métier pour traiter les valeurs aberrantes des features numériques :
Pour les valeurs qui doivent être entre 0 et 100g, une valeur négative ou >100g est aberrante
Un traitement par la méthode interquartile créer définit des outliers mais qui ne sont pas forcément des valeurs aberrantes, mais plutôt atypiques. Par exemple un paquet de sel contient 100g de sel pour 100g de produit, la méthode interquatile proposerait de supprimer ce produit, car très peu de produit ont une valeur de sel >10g pour 100g de produit
La méthode interquartile peut être testée, mais sur des données homogènes, par catégorie de produit (pnns_group_1 par exemple) et comparée à l’approche métier
Pour l’énergie, vérifier sur Internet la valeur maximale possible pour 100g, pour l’utiliser comme seuil de valeur aberrante
Une fois détectées les valeurs aberrantes, 2 approches sont possibles :
Supprimer les lignes correspondantes (produits)
Remplacer ces valeurs par NaN, elles seront retraitées dans l’étape suivante
Autres traitements possibles de détection de valeurs aberrantes :
La somme des ingrédients est > 100g (attention satured_fat est inclus dans fat, idem pour sugar dans carbohydrates)
La valeur satured_fat est supérieure à fat, idem pour sugar et carbohydrates)
Un produit contient au moins N% de NaN parmi ces features numériques (donc impossibilité ensuite de recalculer les données manquantes chapitre suivant)
Milestone 3 : Nettoyage – valeurs manquantes
Livrable :
Notebook de nettoyage, partie traitement des valeurs manquantes
Niveau d’avancement : 60%
Problèmes et erreurs courants :
Erreur d’appliquer mécaniquement des traitements, sans se poser la question de la pertinence métier
Erreur d’utiliser un Iterative Imputer sur des données non corrélées entre elles
Recommandations :
Les traitements précédents ne doivent pas avoir pour conséquence de supprimer toutes les valeurs manquantes (NaN), sinon la compétence de cette étape ne pourra pas être mises en évidence
La stratégie de traitement des valeurs manquantes doit être adaptée à chaque feature en fonction du contexte métier du projet :
Eventuellement choix de supprimer un produit, à éviter au maximum
Remplissage par « 0 » si l’on estime que la saisie est bonne, mais que les produits ont dans cas en réalité une valeur nulle pour la feature : cela peut être le cas de la feature « fiber », car de nombreux produits ne contiennent pas de fibre
Remplissage par la médiane, à condition de le faire sur des produits homogènes, donc par catégorie de produit (pnns_group_1 par exemple)
Remplissage par un IterativeImputer sur les features corrélées entre elles (analyse via heatmap de corrélation), car la base de ce traitement est par défaut une régression linéaire. Par exemple la feature « salt » n’est corrélée à aucune autre feature, donc il n’est pas pertinent de le faire dans ce cas. Par contre les features « energy », « fat », « satured_fat », « sugar », « carbohydrates » ont des corrélations avec certaines des autres features citées, donc sont éligibles à ce traitement
Avantage : cette approche est très rapide à mettre en œuvre
Inconvénient : c’est une boîte noire, il n’y a pas de mesure de la pertinence de ce traitement (pas de scoring)
Utilisation d’autres techniques, notamment de machine learning. Cela peut intéressant pour recalculer le nutriscore et/ou le nutrigrade (CF cours associé, Entraînez votre premier k-NN)
Inconvénient : la démarche est plus lourde à mettre en œuvre
Avantage : un score permet de mesurer la performance du retraitement, et c’est l’occasion de commencer à mettre en œuvre un premier algorithme de machine learning, en préparation du projet suivant…
Milestone 4 : Analyse exploratoire – Analyse uni-variée et bi-variée
Livrable :
Notebook d’analyse exploratoire – partie analyse univariée et bi-variée
Niveau d’avancement : 80%
Recommandations :
Une fois le fichier nettoyé, il est attendu de réaliser une analyse exploratoire complète, même si certaines analyses ont déjà été réalisées pour les besoins du nettoyage sur des données moins nettoyées
Cette analyse exploratoire servira également à valider que le jeu de données est prêt et pertinent pour valider l’idée d’application initiale
Analyse uni-variée :
Features numériques : il est attendu un describe(), des graphiques de type distribution ou boxplot
Features catégorielles : il est attendu des graphiques de type barplot ou camembert
Analyse bi-variée :
Features numériques entre elles : par exemple scatterplot, pairplot, heatmap de corrélation
Feature numérique / feature catégorielle : par exemple feature « fat », avec boxplot selon le nutrigrade (A, B, C, D, E).
Milestone 5 : Analyse exploratoire – Analyse multi-variée
Livrable :
Notebook d’analyse exploratoire – partie analyse multi-variée
Niveau d’avancement : 100%
Recommandations :
ACP – Analyse multi-variée descriptive :
Il est attendu de réaliser un « ébouli » (niveau de variance expliquée par les composantes principales), un cercle de corrélation et une projection des individus
L’ébouli doit montrer que les deux premières composantes principales expliquent environ 60% de la variance
Le cercle de corrélation permet de montrer graphiquement sur chaque plan en 2D les corrélations entre les features et le nutriscore (principalement le plan des 2ères composantes principales F1 et F2, puis F3 et F4 éventuellement)
La projection des individus apporte un complément d’analyse, à condition de colorier les points selon une catégorie (nutrigrade, pnns_group_1), afin de confirmer des regroupements selon ces catégories
ANOVA
Une analyse ANOVA est attendue, par exemple calcul de corrélation entre une feature numérique et une feature catégorielle (eta-square par exemple)
L’étudiant pourra éventuellement réaliser un test statistique (calcul de la p-value).

 
 
 
