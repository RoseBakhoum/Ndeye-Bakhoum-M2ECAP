
# ETUDE SUR LES TENDANCES D'ACHATS DES CLIENTS
 

Notre objectif sera d'étudier le tendance d'achat des clients afin de permettre aux entreprises d'adapter leur espace de vennte 
mais également leur produits proposées à leur clientèle pour booster leur vente. 


### Description des données 

Nous avons choisi un ensemble de variables pour mener notre étude. Parmi lesquelles nous avons 
Suivant la description des données , nous avons :

Customer ID :             Identifiant unique pour chaque client
Age :                      Âge du client
Gender :                   Genre du client (Homme/Femme)
Item Purchased :           L'article acheté par le client
Category :                 Catégorie de l'article acheté
Purchase Amount (USD) :    Le montant de l'achat en USD
Location :                 Lieu où l'achat a été effectué
Size :                     Taille de l'article acheté
Color :                    Couleur de l'article acheté
Season :                   Saison pendant laquelle l'achat a été effectué
Review Rating :            Note donnée par le client pour l'article acheté
Subscription Status :      Indique si le client dispose d'un abonnement (Oui/Non)
Shipping Type :            Type d'expédition choisi par le client
Discount Applied :         Indique si une remise a été appliquée à l'achat (Oui/Non)
Promo Code Used :          Indique si un code promotionnel a été utilisé pour l'achat (Oui/Non)
Previous Purchases :       Le nombre total de transactions conclues par le client au magasin, à l'exclusion de la transaction en cours
Payment Method :           ​​Mode de paiement préféré du client
Frequency of Purchases :   Fréquence à laquelle le client effectue des achats (par exemple, hebdomadaire, bimensuel, mensuel)


# I _ Analyse exploiratoire des données

Aprés l'importation de notre jeu de données, nous avons vérifier si toutes nos variables étaient aux formats. Ensuite nous sommes 
passés à la vérification des données manquantes. Nous avons constaté que notre base ne comporte pas de données manquantes

# II_ Analyse statistique des données

  #  1_ Statistiques descriptives des variables quantitatives 

![image](https://user-images.githubusercontent.com/C:/Users/HP/Pictures/cp.png)
![image](https://github.com/RoseBakhoum/Ndeye-Bakhoum-M2ECAP/edit/main/Exercice.md/cp.png)
![image]("C:\Users\HP\Pictures\cp.png")

Il existe quand meme une différence entre les hommes et les femmes. En effet les femmes sont plus susceptibles de ne pas avoir le diabète que les hommes. Alors que les hommes ont plus de chance d'avoir le diabète que les femmes.

![image](https://user-images.githubusercontent.com/118168338/218112438-046e2b3c-bf50-4952-9cb5-5395f0649984.png)

Il  y'a une relation négative entre l'activité physique au cours de 30 jours et le diabète. En effet , plus une personne fait du sport , moins elle a de chance d'avoir le diabète. 


![image](https://user-images.githubusercontent.com/118168338/218113733-393d9168-c213-46b5-8483-e56002263e55.png)


Il existe une relation positive entre les variables Diabetes et HighChol. Plus une personne a un haut niveau de cholestérol, plus celle-ci a de chance à avoir le diabète.



![image](https://user-images.githubusercontent.com/118168338/218113849-a51e0780-38fb-412e-a63d-bb36430695d6.png)

Il existe un lien positif avec le fait de fumer au moins 100 cigarettes dans sa vie et avoir le diabète. Plus une personne n'a pas fumé 100 cigarettes dans sa vie , plus elle a de chance de pas avoir le diabète.


   #2_Statistiques descriptives des variables quantitatives 

Pour le coup , nous avons une seule variable quantitative qui est BMI soit l'indice de masse corporelle.

Dans notre échantillon , la moyenne de l'indice de masse corporelle est de 29,85. La valeur minimun est de 12 et la valeur maximun est de 98. 25% des personnes interrogées ont un IMC inférieur ou égale à 25 et les 75% ont ce dernier qui inférieur ou égal à 33. La moitié des personnes interrogées ont un IMC inférieur ou égal à 29. On peut dire que les personnes intérrogées sont généralement en situation de surpoids.

Nous regardons ensuite la distribution de la variable 

![image](https://user-images.githubusercontent.com/118168338/218115191-a8ba0d4b-d43a-4f83-bc3e-b152016b0c24.png)

Nous avons une distribution asymétrique de la variable BMI. L'indice de masse corporelle a une asymétrie positive. Sa distribution est leptokurtique.

Nous avons aussi regardeé le lien entre la variable BMI et la variable Diabetes. 

![image](https://user-images.githubusercontent.com/118168338/218115935-aedfec8c-1f90-46cb-acc2-156d8fb97fa5.png)

La probabilité d'avoir le diabète est plus élevée si l'IMC est entre 25 et 50. De manière générale les diabétiques ont un fort IMC.

Nous voulions savoir si la variable BMI possédait des valeurs aberrantes car ces dernières peuvent pertuber la prédiction de la variable target.
Pour cela , le boxplot a été utilisé . 

![image](https://user-images.githubusercontent.com/118168338/218117787-c9c4063d-c4a5-4218-a66e-79aac7cf1aa9.png)

La variable BMI possède des valeurs aberrantes suivant le boxplot. On constate que ces dernières ont tendance à etre supérieures à 50. Ainsi , on décide de supprimer les valeurs supérieures à 50. En refaisant les statistiques descriptives de la variable , on constate que cette dernière n'a pas beaucoup changée. C'est la valeur maximale de l'indice et sa la valeur médiane de cette dernière qui sont passées respectivement de 49 et 28. 


  
   #3_Statistiques descriptives des variables qualitatives
   
 On fait les statistiques descriptives de chaque variable qualitatives. Ensuite nous avons essayer de voir un lien entre deux variables quantitatives
   
   
Pour la variable Sex , Il y'a plus de femmes que d'hommes. Elles sont au nombre de 38.386 alors que les hommes sont au nombre de 32.306. Pour l'age , la majorité des personnes interrogées se trouvent entre 65 et 69 ans (10856). Elle est suivie des personnes agées de 60 à 64 ans au nombre de 10.112 personnes. Les jeunes de 18 à 24 ans sont en minorité (979 personnes). De manière générale , ce sont les personnes agées de 50 ans à 74 ans qui sont les plus nombreuses dans nos observations. On constate aussi que la majorité des personnes ont fumé 100 cigarettes dans leur vie . Vu qu'on une population assez viellissante , c'est normal que le nombre de personnes ayant un un fort niveau de cholestérol soit plus nombreux. On utilise le meme procédé pour les autres variables .


![image](https://user-images.githubusercontent.com/118168338/218120425-f1b36ff1-9510-4b76-9d99-d1e629381e5c.png)

Le graphique ci-dessus montre la relation qu'il y'a entre les variables Sex et Smoker. On constate que ,parmi les fumeurs , ce sont les hommes qui fument un peu plus que les femmes. Dans le groupe des non fumeurs , la majorité des personnes qui ne fument pas sont des femmes. 

Vu que certaines variables explicatives sont dépendantes entre elles , nous allons appliquer le test de khi2 pour vérifier la dépendance des variables explicatives qualitatives. En effet , c'est pour éviter un risque de multicolinéarité qui peut pertuber la prédiction de la variable Diabetes. L'hypothèse nulle du test suppose que les variables sont indépendantes et dans l'hypothèse alternative suppose que les variables sont dépendantes. Si la pvalue du test est inférieur à 0,05 alors les variables sont dépendantes.Pour le test , nous créons beaucoup de tableaux croisées entre deux variables qualitatives . Ensuite nous appliquons la fonction du KHI sur le tableau croisée et nous observons la pvalue. De manière générale , presque toutes les variables explicatives qualitatives sont dépendantes entre elle. Cependant les variables CholCheck et Smoker ne sont pas dépendantes entre elles. Pour cela , nous décidons de garder les variables Smoker , BMI et CholCheck comme variables explicatives. 


# III_Préparation de la base de données pour les prédictions

Nous allons passer à la prédiction . Mais avant tout , nous recodons la variable Diabetes en int32 pour pouvoir faire la prédiction. Vu que notre variable à prédire est une variable binaire alors nous allons passé à des classifications . Pour cela 4 méthodes sont sélectionnées. 
La régression logistique : 

Cette méthode est avant tout une méthode de classification binaire qui peut prendre en compte les variables quantitatives et les variables qualitatives.
Elle est facile à interpréter . 

Les SVM (Support Vector Machine) : 

Les SVM sont une classe d'algorithmes d'apprentissage . Ils ont pour but de truver une frontière de décision qui permet de séparer les valeurs d'une variable afin de mieux les classer soit de manière linéaire ou non linéaire. Dans notre projet , nous utiliserons les SVM linéaire.Pour cela , nous avons le Linear SVC , le SVC avec le noyau linéaire et le SGDClassifier.

Nous séparons notre base de données initiale en une base prenant en compte les deux modalités de notre variable target , soit 0 et 1. Cette dernière est appelée bin_diabetes. Cette meme base sera divisée en deux bases de donées d'entrainement et en deux bases de données test. Après nous devons standardiser nos données , puisque ces dernières n'ont pas la meme échelle. 

Ensuite , nous pouvons commencer les prédictions de chaque modèle. 


# IV_Différentes méthodes de prédiction

Comme nous l'avons dit précedemment , nous allons faire des prédiction avec la régression logistique , le Linear SVM , le SVM avec le Kernel linéaire et 
le SGDClassifier .

  # a_Régression logistique 
  
  Unknown.png![image](https://user-images.githubusercontent.com/118168338/218143871-70a4d112-3808-47ad-b98a-28397624dff2.png)
  
 Suivant la matrice de confusion du modèle logistique , la prédiction ecxate du  nombre de personnes n'ayant pas le diabète est de 7144 .Celle de ceux qui ont le diabète est de 6312 . Ce qui nous donne un accuracy de 64%. Ce qui veut dire que le modèle logistique prédit correctement la variable Diabetes à 64%. 


# b_ Linear SVM

![image](https://user-images.githubusercontent.com/118168338/218144265-a190a804-8501-4ef2-a11a-057de38e1a9f.png)

Pour le modèle Linear SVM , On obtient la matrice de confusion.La prédiction ecxate du nombre de personnes n'ayant pas le diabète est de 7142 .Celle de ceux qui ont le diabète est de 6315 . Ce qui nous donne un accuracy de 64%. Ce qui veut dire que le modèle LinearSVC possède une bonne prédiction de 64%.



# c_ SVM avec kernel linear

![image](https://user-images.githubusercontent.com/118168338/218152561-f213ab06-0961-4061-ae9b-507721d67784.png)

Pour le modèle SVM avec le noyau linéaire , la prédiction ecxate du nombre de personnes n'ayant pas le diabète est de 7139 .Celle de ceux qui ont le diabète est de 6324 . Ce qui nous donne un accuracy de 64%. Ce qui veut dire que le modèle SVC avec le noyau linéaire prédit correctement  la variable Diabetes à 64%.


# d_ SGD classifier

![image](https://user-images.githubusercontent.com/118168338/218152864-e3b1f961-88ea-4602-aa33-89c04654293f.png)

Pour le modèle SGDClassifier, la prédiction ecxate du nombre de personnes n'ayant pas le diabète est de 7144. .Celle de ceux qui ont le diabète est de 6312 . Ce qui nous donne un accuracy de 64%. Ce qui veut dire que le modèle SGDClassifier prédit correctement à la variable Diabetes à 64%. 

Nous nous retrouvons avec les 4 modèles SVM qui ont des accracy égaux . Ceci n'est pas encore suffisant. Pour faire notre choix de modèle , nous allons regarder l'évolution des accuracy_scores en fonction de folds.

![image](https://user-images.githubusercontent.com/118168338/218153344-12b022d6-3b2d-4d11-bf99-9959439c9c70.png)

On constate que les méthodes ont le meme taux de bonnes prédictions qui est de 64%. Cependant nous choisissons le modèle logistique car ve dernier possède la plus grande accuracy et aussi il a le plus petit std qui de 0,00430. Comparé aux autres modèles , il a moins de chances de faire un surapprentissage. Nous voulions appliquer l'agorithme Gridsearch pour améliorer notre modèle. Malheureusement , nous pouvons pas appliquer l'algorithme sur notre ordinateur. Donc nous allons passer à l'analyse du modèle choisi.


# V_ Analyse du modèle choisi

Nous constatons que la moyenne des accuraccy de la base d'entrainement et celle de la base test sont respectivement de 0.6451612903225806  et de 0.6446605662817995. Vu que les scores des deux bases sont presques pareilles , il n'ya pas de risque de surapprentissage. 
Les variables explicatives possèdent chacune , une relation positive avec la variable à prédire suivant leur coefficient. En effet , Plus une personne vérifie son cholestérol dans 5 ans , plus cette dernière a la chance d'avoir le diabète (0.28). C'est la meme chose pour la variable Smoker(0.18). Plus l'indice de masse corporelle d'une personne augmente , plus cette dernière a la chance d'avoir le diabète(0.7). 














