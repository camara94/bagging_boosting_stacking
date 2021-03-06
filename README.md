# Ensemble Learning: Bagging Boosting Stacking

Python Machine Learning en français vous enseigne les techniques d'Ensemble Learning : Bagging Boosting et Stacking, qui permettent de développer les modèles de machine learning les plus puissants au monde, comme l'algorithme de Random Forest.

## Ensemble Learning
En statistique et en apprentissage automatique, l'apprentissage ensembliste utilise plusieurs algorithmes d'apprentissage pour obtenir de meilleures prédictions.

Par exemple<br> l'ensemble de méthodes **bagging**, **boosting** et les **forêts aléatoires** est un exemple d'apprentissage ensembliste.

## Bagging
Le **bootstrap aggregating**, également appelé **bagging** (de bootstrap aggregating), est un meta-algorithme d'apprentissage ensembliste conçu pour améliorer la stabilité et la précision des algorithmes d'apprentissage automatique. Il réduit la variance et permet d'éviter le surapprentissage. Bien qu'il soit généralement appliqué aux méthodes d'arbres de décision, il peut être utilisé avec n'importe quel type de méthode. Le bootstrap aggregating est un cas particulier de l'approche d'apprentissage ensembliste.

![image 11](images/11.png)

![image 12](images/12.png)

![image 13](images/13.png)

* Exemple<br>
Avec Scikit-learn, il est simple de produire de tels modèles baggés, par exemple :
 1. Un bagging d’arbres de décision sera généré sur scikit-learn ou weka à partir des classes suivantes:
sklearn.ensemble.RandomForestClassifier(n_estimators=10)
2. weka.classifiers.meta.Bagging

   ![image 1](images/1.png)

## Boosting
Le boosting est un domaine de l'apprentissage automatique (branche de l'intelligence artificielle). C'est un principe qui regroupe de nombreux algorithmes qui s'appuient sur des ensembles de classifieurs binaires : le boosting optimise leurs performances.

Le principe est issu de la combinaison de classifieurs (appelés également hypothèses). Par itérations successives, la connaissance d'un classifieur faible - weak classifier - est ajoutée au classifieur final - strong classifier.

On appelle apprenant faible un algorithme qui fournit des classifieurs faibles, capables de reconnaître deux classes au moins aussi bien que le hasard ne le ferait (c’est-à-dire qu'il ne se trompe pas plus d'une fois sur deux en moyenne, si la distribution des classes est équilibrée). Le classifieur fourni est pondéré par la qualité de sa classification : mieux il classe, plus il sera important. Les exemples mal classés sont boostés pour qu'ils aient davantage d'importance vis-à-vis de l'apprenant faible au prochain tour, afin qu'il pallie le manque.

![image 14](images/14.png)

* Exemple:  
Scikit-learn par exemple propose par défaut Adaboost avec :
  1. sklearn.ensemble.AdaBoostClassifier(n_estimators=100)
  2. weka.classifiers.AdaBoostM1

    ![image 2](images/2.png)

## Bagging VS Boosting

![image 15](images/15.png)

## Stacking

Le stacking (ou dit parfois blending) est un procédé qui consiste à appliquer un algorithme de machine learning à des classifieur générés par un autre algorithme de machine learning.

D’une certaine façon, il s’agit de prédire quels sont les meilleurs classifieurs et de les pondérer. Cette démarche a l’avantage de pouvoir agréger des modèles très différents et d’améliorer sensiblement la qualité de la prédiction finale, le challenge NetFlix à 1 million $ en est la meilleure preuve.

![image 16](images/16.png)

## Proverbe

![image 3](images/3.png)

Autrement dit

![image 4](images/4.png)

Exemple en Machine Learning

![image 5](images/5.png)

## La Loi des Grands Nombres

![image 6](images/6.png)

## Attention pour la Loi des Grands Nombres

![image 7](images/7.png)

![image 8](images/8.png)

![image 9](images/9.png)

![image 10](images/10.png)

## Comment choisir: le modèle d'ensemble learning

* Lorsqu'on observe l'overfitting sur la somme de nos modèles alors On utilise le **Boosting**
* Lorsqu'on observe l'under-fitting sur la somme de nos modèles alors On utilise le **Bagging**

## Ressources

1. [https://fr.wikipedia.org/wiki/Apprentissage_ensembliste](https://fr.wikipedia.org/wiki/Apprentissage_ensembliste)
2. [https://fr.wikipedia.org/wiki/Bootstrap_aggregating](https://fr.wikipedia.org/wiki/Bootstrap_aggregating) 
3. [https://fr.wikipedia.org/wiki/Boosting](https://fr.wikipedia.org/wiki/Boosting)
4. [https://www.youtube.com/watch?v=7C_YpudYtw8](https://www.youtube.com/watch?v=7C_YpudYtw8)
5. [https://blog.octo.com/les-methodes-ensemblistes-pour-algorithmes-de-machine-learning/](https://blog.octo.com/les-methodes-ensemblistes-pour-algorithmes-de-machine-learning/)