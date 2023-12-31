# Indentation 2023 : Post Traitement des essais d'indentation

## Remarques introductives

* Ce tutoriel est pensé pour durer 2h.
* Tous les outils qu'il utilise sont libres et donc gratuits. 
Le mieux est donc de les installer sur votre machine pour vous les approprier.
* Ce dépôt contiendra tous les fichiers que nous produirons pendant la formation.

## Contexte

Dans ce tutoriel, nous allons utiliser la librairie Indentoolbox qui a été développée suite à nos discussions à Indentation2021 à Lorient.
Pour commencer, vous invite à regarder le [dépôt de la librairie](https://gitlab.com/indpp/indentoolbox) et [sa documentation](https://indentoolbox.readthedocs.io/en/latest/).
Cette libraire est développée pour la communauté et, à terme, elle sera développée par la communauté.
Elle doit donc répondre à vos besoins et vous devez faire savoir si ce n'est pas le cas.


## Instructions

Vous aurez plusieurs possibilités pour travailler pendant la formation:

* Sur votre machine personnelle (préférable): si vous choisissez cette option, vous devez installer certains logiciels avant la formation:
    * Anaconda: https://www.anaconda.com/
        * Attention: sous Windows, il faudra installer pour votre utilisateur et ajouter Anaconda à votre "PATH" comme montré ci-dessous:
        ![](images/anaconda_install_1.png)
        ![](images/anaconda_install_2.png)
        
        * Sous Linux: miniconda suffira ou tout autre gestionnaire d'environnements virtuels Python.

    * Un client Git:
        * Sous Windows: https://git-scm.com/
        * Sous Linux: vous l'avez de base normalement, à vérifier.
    * Vscode: https://code.visualstudio.com/
    * Suivre les instructions d'installation du module IndenToolbox "Standard user" ici: https://gitlab.com/indpp/indentoolbox#for-standard-users
* Sur une machine de la salle informatique ou aura lieu la formation: cette solution est moins préférable mais sera disponible si vous n'arrivez pas ou ne pouvez pas installer les logiciels sur votre machine.

## Données

Des datasets d'essais d'indentation sont disponibles à [ce lien](https://drive.google.com/drive/folders/169cgLeRt96IWq4aN9yQJpiF7VQ2WXWEB?usp=sharing).
Vous avez aussi produit des données d'indentation lors de la session expérimentale, vous pouvez les utiliser si vous disposez d'un export en format `txt`.

Les données expérimentales fournies avec ce tutoriel sont les suivantes:

|                 Dossier                |         Matériau         | Coefficient de Poisson $\nu$ | Module de Young $E$ [GPa] |
|:--------------------------------------:|:------------------------:|:----------------------------:|:-------------------------:|
| 2011-06-28_Hysitron_TI950_Fused_Quartz |   Silice pure (amorphe)  |             0.16             |             72            |
|      2014_Hysitron_TI950_Tungsten      |       Tungsten pur       |              0.28            |            400            |
|   2011-05_BMG_Fe41Co7Cr15Mo14C15B6Y2   | Verre métallique base Fe |             0.337            |           225.0           |
|      2011_05_BMG_Zr50Cu40Al10-400C     | Verre métallique base Zr |             0.359            |            94.8           |


Les essais ont été réalisés sur une machine Hysitron TI950 avec une point Berkovich en diamant.

## Etapes du tutoriel

1. Si ce n'est pas fait, installer les logiciels.
2. Créer un notebook avec Jupyter Lab et, en vous inspirant du tutoriel sur le *pre-processing* dans la documentation de IndentoolBox, réaliser un pré-traitement de vos essais. Sauvegardez vos *batches* avec un nom explicite.
3. Réalisez la démarche proposée dans le tutoriel dédié au post-traitement. Dans le cas de la silice, vérifiez que le module que vous obtenez est correct.
4. Dans le cas du tungsten, appliquez les méthodes inverses de proposées dans IndentoolBox pour les métaux cristallins. 
5. Ajoutez toute étape qui vous semble pertinente en tenant compte de vos habitudes d'expérimentateur.

## Objectifs

* [ ] Découverte de l'outil `IndentoolBox`.
* [ ] Installation et configuration (suivre les instructions de la documentation).
* [ ] Choix de données à traiter.
* [ ] Création d'un notebook avec Jupyter Lab.
* [ ] *Pre-processing* basique de vos données.
* [ ] *Post-processing* de celles-ci.
* [ ] Discussion sur la suite et la manière de procéder pour faire vivre/évoluer l'outil.

