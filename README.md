# Mammals_space

Les données sont disponibles à ce lien : https://www.kaggle.com/datasets/gwendaltsang/cropped-dog-breeds

Ces données s'inscrivent dans un projet concernant la génération d'images intermédiaires (par combinaisons affines / linéaires entre deux vecteurs)

Un bon exemple est donné au lien suivant :

https://stylegan-nada.github.io/

Voir aussi l'article de [NITZAN et al. (2020) intitulé _Face Identity Disentanglement via Latent Space Mapping_](https://arxiv.org/abs/2005.07728)

Ce qu'il y a d'intéressant, dans cet article, tient à ce qu'ils parviennent à séparer l'identité du visage (les propriétés qui restent fixes) des attributs qui peuvent être variables. Cela permet ensuite, par exemple, de modifier les attributs variables (par exemple le sourire, la position du visage) sans toucher aux propriétés stables qui constituent l'identité du visage.

Le projet consiste à entraîner un réseau de mapping (M) pour exploiter l'espace latent d'un générateur StyleGAN pré-entraîné et gelé. Le système apprend à combiner la race d'une image source I_id avec la pose d'une autre image I_attr. La préservation de la race est assurée par une perte d'identité calculée à l'aide d'un classifieur de races pré-entraîné et gelé (frozen), permettant ainsi un transfert d'attributs contrôlé.


Quelques ensemble de photos de mammifères.

https://www.kaggle.com/datasets/crawford/cat-dataset/data

https://github.com/AtharvaTaras/Cat-Images-Dataset

Celui-ci semble particulièrement pertinent pour faire un clustering :

https://www.kaggle.com/datasets/borhanitrash/cat-dataset/data

Nous souhaiterions nous inspirer de :

https://www.kaggle.com/discussions/accomplishments/503087
https://www.kaggle.com/code/alfredkondoro/pytorch-mnist-vae-cnn
https://www.kaggle.com/code/alfredkondoro/pytorch-mnist-vae


https://www.kaggle.com/code/fazilbtopal/variantional-autoencoders-vae

https://www.kaggle.com/code/alincijov/cnn-vae-handwritten-math-symbols-tf

L'une des finalités serait la _feature extraction_ , à cet égard, voir par exemple : https://arxiv.org/pdf/2204.07924

