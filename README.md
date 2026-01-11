![Alt text](images/image_3.jpg)


# Mini_Projet_Pandas

**Professeur :** Dr. Evens TOUSSAINT  

**Étudiants :**  
- Jameson PIERREVILLE  
- Fabrice HERARD  
- Steve CALIXTE

## Presentation
![Alt text](images/download_3.WEBP)

Nous occupons le rôle de Data Analyst au sein de l’entreprise EduMart, une boutique spécialisée dans la vente de cours, livres, logiciels, crédits cloud, ordinateurs portables et accessoires. Notre tâche consistent à nettoyer et analyser les données de ventes ainsi que le comportement des clients (retours, avis, etc.) à l’aide de Pandas.


## The Data
![Alt text](images/download_4.WEBP)

Notre jeu de données est composé de trois fichiers CSV décrivant les clients, les produits et les transactions de l’entreprise EduMart. Les données vont de la période allant de 2024 à 2025. Le dataset qui enregistre les transactions comptent environ 2200 lignes. 





## Methode
Pour réaliser ce travail, nous utiliserons les outils offerts par _Python_, principalement la bibliothèque _pandas_, qui nous permettra de manipuler les _DataFrames_. Dans un premier temps, nous mènerons une _analyse exploratoire des données_ afin d’identifier, entre autres, la présence de valeurs manquantes.

Dans un deuxième temps, nous traiterons ces différentes anomalies à l’aide de techniques de _nettoyage et de préparation des données_. Enfin, nous exploiterons les données en utilisant des _méthodes statistiques_ et des _visualisations graphiques_ afin d’en extraire des informations pertinentes.

Comme outil collaboratif, nous utiliserons _GitHub_, qui nous permettra d’héberger notre projet, mais aussi de collaborer efficacement et en temps réel sur la production et la révision du code.




## Analyse & Resultat
### Rapport d’audit  sur la qualité des données.
Après l’importation des datasets customers, products et order_lines, plusieurs anomalies et valeurs manquantes ont été identifiées:   
- La colonne age contient des valeurs manquantes et des entrées non numériques (unknown).
- Des valeurs manquantes sont présentes dans gender, city et review_score.
- discount_pct est parfois stocké sous forme de texte.
- quantity contient des valeurs négatives ou nulles.
- delivery_days contient des valeurs extrêmes.
- Les dates sont stockées en texte.

###  Rapport d’audit des données : analyse des jointures
- Vérification des clients non trouvés dans la table order_customers : certaines informations manquent.  
- Nombre de ventes associées à des clients manquants : 159.  
- Contrôle des écarts sur le montant brut (gross_amount) a identifié 6 lignes suspectes.  
- Certaines clés primaires apparaissent dans d’autres colonnes similaires, ce qui peut créer des doublons ou des ambiguïtés.  
- Des suffixes ont été ajoutés pour identifier clairement à quelles données appartiennent ces lignes, facilitant le suivi et la correction.