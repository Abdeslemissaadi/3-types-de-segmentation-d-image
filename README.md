# 3-types-de-segmentation-d-image

Ce projet compare 3 types de segmentation d'image avec des modèles de deep learning pré-entraînés (sur COCO), pour montrer la différence entre chaque approche :

Segmentation panoptique (Panoptic FPN) → segmente à la fois les objets individuels ET le fond (route, ciel, herbe...)
Segmentation d'instance (Mask R-CNN) → détecte et délimite chaque objet individuellement (ex : chaque personne séparément)
Segmentation sémantique (DeepLabV3) → classe chaque pixel par catégorie, sans distinguer les instances (tous les "chats" ont la même couleur, peu importe combien il y en a)

Déroulé du script : upload d'une image → passage dans chacun des 3 modèles → affichage visuel du résultat de chaque méthode côte à côte pour comparaison.

Technologies :

Detectron2 (Facebook AI Research) → panoptique + instance
Torchvision (DeepLabV3) → sémantique
PyTorch, OpenCV, Matplotlib
Exécution sur Google Colab (CPU)
