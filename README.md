# Projet 3 : Compréhension du comportement des utilisateurs

- Vous êtes un data scientist dans une entreprise de développement de jeux vidéo.

- Votre dernier jeu mobile comporte deux événements que vous souhaitez suivre : achat d'une `épée` et `rejoindre une guilde`.

- Chacun de ces événements a des métadonnées caractéristiques de ces événements (par exemple, type d'épée, nom de la guilde, etc.).


## Tâches

- Instrumentez votre serveur API pour enregistrer les événements dans Kafka.

- Montez un pipeline de données pour capturer ces événements : utilisez Spark Streaming pour filtrer certains types d'événements depuis Kafka, puis enregistrez-les dans HDFS au format Parquet pour les rendre disponibles à l'analyse via Presto.

- Utilisez Apache Bench pour générer des données de test pour votre pipeline.

- Produisez un rapport d'analyse où vous fournissez une description de votre pipeline et une analyse de base des événements.

Utilisez un notebook pour présenter vos requêtes et résultats. N'oubliez pas que ce notebook doit être adapté à une présentation pour quelqu'un de votre entreprise qui devra prendre des décisions basées sur vos recommandations.

Il est entendu que les événements dans ce pipeline sont des événements générés, ce qui les rend difficiles à relier à des décisions commerciales réelles. Cependant, nous souhaitons que les étudiants démontrent leur capacité à construire ce pipeline de bout en bout, ce qui inclut la génération initiale de données de test ainsi que la soumission d'un rapport sous forme de notebook comprenant au moins une analyse simple des événements.


## Options

Il existe de nombreuses options avancées pour ce projet. Voici quelques façons d'aller plus loin que les bases que nous couvrirons en classe :

- Générez et filtrez davantage de types d'événements. Il existe de nombreux autres événements que vous pourriez capturer pendant le jeu.

- Améliorez l'API en utilisant des verbes HTTP supplémentaires comme `POST` ou `DELETE` et en acceptant des paramètres pour les événements (par exemple, les événements d'achat pourraient accepter le type d'épée ou d'objet).

- Connectez un moteur de stockage basé sur clé utilisateur, comme Redis ou Cassandra, à Spark afin de suivre l'état de l'utilisateur pendant le jeu (par exemple, l'inventaire ou la santé de l'utilisateur).
