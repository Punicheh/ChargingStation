# ChargingStation

# Analyse de la Répartition des Infrastructures de Recharge en France

## Introduction

Dans le cadre de notre projet, nous avons travaillé sur la problématique suivante : **La répartition des infrastructures de recharge sur le territoire correspond-elle à une logique de distribution de la population et de trafic routier ?**. Cette question nous a guidés à travers l’analyse de données disponibles sur les bornes de recharge électrique, afin de comprendre la cohérence entre le nombre de bornes, la densité de la population, et le trafic routier à travers les différents départements de France.

Notre objectif était de vérifier si la répartition des bornes de recharge suit logiquement la densité de la population et le trafic routier, permettant ainsi d'évaluer l'efficacité de l'infrastructure de recharge au regard de l'utilisation potentielle par les habitants et les usagers de la route.

## Cible : Professionnels de l'Installation de Bornes

Notre analyse s'adresse principalement à **tous les professionnels souhaitant installer des bornes de recharge électrique**. Cela inclut non seulement les entreprises spécialisées dans l'installation d'infrastructures de recharge, mais aussi les collectivités, les gestionnaires d'infrastructures, les promoteurs immobiliers, et tout autre acteur souhaitant participer au développement du réseau de bornes en France.

Notre étude leur fournit des **indicateurs clairs sur les besoins par département**, en tenant compte à la fois de la **densité de population, du trafic routier**, ainsi que du **nombre de bornes existantes et de leur localisation exacte** par département. Ces données permettent de mieux cibler les zones à fort potentiel qui manquent encore d'infrastructures adaptées, optimisant ainsi les décisions quant aux localisations prioritaires pour de nouvelles installations. L'objectif est de faciliter une **planification stratégique**, afin d'améliorer la couverture du territoire en infrastructures de recharge tout en répondant de manière adéquate aux besoins des utilisateurs finaux.

## Méthodologie

### Analyse des Bornes de Recharge par Population et Trafic

Dans un premier temps, nous avons décidé de **réaliser une analyse du nombre de bornes de recharge en fonction de la population et du trafic annuel**. L’idée principale était de vérifier si le nombre de bornes de recharge disponible correspondait au besoin des habitants et à la circulation routière dans chaque département.

Pour ce faire, nous avons commencé par calculer le nombre total de bornes de recharge électrique par département. Les données comprenaient le **nombre de bornes de recharge, la population par département**, ainsi que les informations relatives au **Trafic Moyen Journalier Annuel (TMJA)**.

### Formulation d'un Ratio Combiné

Nous avons ensuite développé une formule permettant de **combiner les ratios des bornes par rapport à la population** et **par rapport au trafic routier**. Ce ratio combiné nous permet d’obtenir une vue d’ensemble plus nuancée, qui prend en compte à la fois la densité démographique et la charge potentielle liée au trafic routier.

Le calcul de ce ratio combiné a été intégré dans un fichier Excel, que nous avons utilisé pour **synthétiser et visualiser** nos résultats sous forme de carte et de tableaux. Ce travail nous a permis d'identifier les régions sous-équipées ou suréquipées, en tenant compte de l’ensemble de ces facteurs.

### Calcul des Indicateurs de Base

1. **Bornes par habitant** :
   Cette mesure nous indique combien de bornes de recharge sont disponibles pour chaque habitant dans un département.
   - **Formule** : `Nombre de bornes / Population du département`

2. **Bornes par trafic** :
   Cela montre combien de bornes sont disponibles par rapport au trafic moyen journalier annuel (TMJA).
   - **Formule** : `Nombre de bornes / TMJA`

### Calcul du Ratio Combiné

Pour combiner ces deux indicateurs (bornes par habitant et bornes par trafic), nous avons procédé à une normalisation :

1. **Normalisation des ratios** : Pour chaque indicateur, nous divisons chaque valeur par la valeur maximale de cette colonne. Cela permet de ramener toutes les valeurs dans une échelle de 0 à 1.
   - **Formule pour la normalisation** : `Valeur actuelle / Valeur maximale de la colonne`

2. **Moyenne des valeurs normalisées** : Ensuite, nous faisons la moyenne des deux valeurs normalisées pour obtenir un ratio combiné.
   - **Formule pour le ratio combiné** : `(bornes_par_habitant_normalisé + bornes_par_trafic_normalisé) / 2`

3. **Conversion en Pourcentage** : Le ratio combiné est ensuite multiplié par 100 pour obtenir un pourcentage. Cela permet de mieux interpréter le niveau de couverture.
   - **Formule pour le pourcentage** : `Ratio combiné * 100`

## Visualisation des Résultats

Pour rendre les résultats plus accessibles et faciliter l'interprétation des données, nous avons réalisé une carte interactive représentant le ratio combiné (%) des bornes de recharge par habitant et par trafic. Cette carte permet une visualisation claire de la répartition des bornes à travers les différents départements de France.

### Carte du Ratio Combiné

[Relation entre Population, Trafic et Couverture en Bornes de Recharge par Département](https://macarte.ign.fr/carte/9AaMOZ/Analyse-des-Opportunites-de-Deploiement-des-Bornes-de-Recharge-Electriques-en-France)

### Feuille de calcul 

[Feuille de calcul Google Sheets des Données de Bornes de Recharge](https://docs.google.com/spreadsheets/d/1KpUIzjNI_tAW0Pn3cikmtc41abmtECPA/edit?usp=sharing&ouid=108501590314128773627&rtpof=true&sd=true)

## Problèmes Rencontrés

Nous avons rencontré certaines difficultés au cours de l'analyse des données. Le **TMJA** n’est pas 100% fiable étant donné que les informations ne sont pas à jour et datent de 2019. De plus, il manque certaines informations, comme pour le département 8 qui ne possède aucune valeur concernant son TMJA, en raison de données incomplètes ou peu claires dans les sources disponibles.

## Conclusion

Grâce à cette analyse, nous avons pu mieux comprendre la répartition des infrastructures de recharge en France. Elle a mis en lumière des disparités régionales importantes, suggérant que certains départements sont potentiellement sous-équipés, tandis que d'autres semblent avoir une bonne densitée de borne par rapport à la population et au trafic routier.

Ces résultats montrent l’importance d’une **planification stratégique des infrastructures de recharge**, pour mieux aligner les besoins des habitants et des usagers de la route avec l’offre de recharge disponible. La visualisation sous forme de carte et de tableau nous a permis de simplifier l'interprétation des données pour un public plus large.

Nous prévoyons d'approfondir cette analyse en examinant des facteurs supplémentaires, tels que la distribution des types de véhicules électriques, la localisation des autoroutes et grandes routes, et les politiques régionales en matière de transition énergétique.

> Nous restons ouverts à vos commentaires et suggestions pour affiner notre analyse et améliorer la qualité des infrastructures de recharge en France.

