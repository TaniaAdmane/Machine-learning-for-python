# Machine-learning-for-python

La data de la ville de philadelphie seulement se trouve ici : 
https://drive.google.com/drive/folders/1TGKSyMR1O96ClNZo47HqJ_w3h1SAo8lZ?usp=sharing


lire papier BERTopic: Neural topic modeling with a class-based TF-IDF procedure ,qui resume bien la structure a suivre 

Etapes 


1) Traitement des données (gros morceau)

    A) données NLP (Sbert est le meilleur outil de tout ce que j'ai cherché)
    B) images (trouver un moyen d'exploiter les images, voir ce qui peut se faire pas trop difficilement et sans GPU)
    C) data qui existe deja 

==> Dead line : 30/12

2) selection des features pertinantes et reduction dimensionnel (tres important aussi)
=>Scaling procedure dans le papier Harini Sureshi et Nick Locascio peut etre interessant

==> Dead line 01/01


4) clusterisation (on test plusieurs algorithmes de clusterisation maybe: K-means, Clustering hiérarchique,DBSCAN ou HDBSCAN,Gaussian Mixtures) avec cross validation pour choisir les hyperparametres
==> Dead line 03/01

5) validations des clusters (silhouette / Davies-Bouldin / stabilité bootstrap) (trouver un papier dessus)
==>Dead line 04/01

6) labelisation des clusters avec td-idf comme dans le papier bertopic. mais apres a voir si ca va nous sortir ce que l'on veut. faudra trouver comment associer un restaurant "attrape touriste" au retour que on a eu avec td-idf
idee : on complete le td-idf avec une exploratiosn manuelle des features en analysant les differentes features du cluster. c'est pour ca qu'il faut faire une bonne selection de features de base. (par exemple « attrape-touristes », « pépites méconnues », « commerces utilitaires »)
(chercher d'autres idées, maybe voir ce qui se fait en etat de l'art)
==> Dead line : 06/01

1 jour de marge 

Dead line : 7 janvier 