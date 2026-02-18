# Classification_Pneumonie_TransferLearning

Dans cet exercice, nous avons utilisé un réseau de neuronnes à convolution à 16 couches pré-entraîné (VGG16) afin de classer des cas de radiologie thoraciques pour déterminer des cas de pneumonies et des cas sains. Ce modèle pourrait permettre d'assister les radiologues dans le diagnostic de la pneumonie et serait utilisable en production par une clinique, un hôpital ou un institut de santé.
Le but de ce projet est d'utiliser le **Transfer Learning** afin d'obtenir des résultats les plus probants possible.

L'utilisation et la compréhension du Transfer Learning est primordial, en effet les données médicales sont rares et protégées or nous devons avoir une très grande base de données pour pouvoir entraîner un modèle efficace.
Le modèle VGG16 a été pré-entraîné sur "ImageNet" (environ 14 millions d'images diverses), ainsi le modèle est expert pour déterminer des géométries basiques tels que des lignes, courbes, textures etc. Avec le transfer learning, nous ré-utilisons un modèle déjà expert dans son domaine (le traitement d'image) pour l'entraîner uniquement sur des images de poumons.
Ainsi, l'entraînement sur quelques milliers de radios thoraciques (en gelant les couches inférieures et en rajoutant notre classificateur) ne prend que quelques minutes et n'est ni coûteux, ni energivore de part le faible nombre de données et en découle d'excellents résultats sur la classification de pneumonies et de cas sains.

https://github.com/eygann/Classification_Pneumonie_TransferLearning/blob/main/classificationPneumonies.ipynb
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]


