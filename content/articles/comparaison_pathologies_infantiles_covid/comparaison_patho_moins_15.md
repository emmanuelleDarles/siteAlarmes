+++
author = ["Vincent Pavan", "Lana Gitrun"]
categories = ["COVID19"]
date = "2021-04-02"
description = "Comparaison des taux d'hospitalisation des pathologies fréquentes par rapport à la Covid19 chez les enfants" 
featured = "pathologie_moins_15ans.png"
featuredalt = "Pic 3"
featuredpath = "/articles/comparaison_pathologies_infantiles_covid/img/"
title = "le Covid19 et les enfants"
type = "post"
+++

## Introduction

Ce document présente une comparaison de la sévérité des pathologies
pédiatriques courantes (grippe, gastro-entérite, pneumopathie,
bronchiolite et asthme) par rapport au Covid19 chez les enfants de moins
de 15 ans.

**Cette étude est entièrement reproductible. L'ensemble du code (script RMarkdown et les données) est téléchargeable :**
- [Fichier de données](/articles/comparaison_pathologies_infantiles_covid/files/patho.xlsx) 
- [Script RMarkdown avec code source](/articles/comparaison_pathologies_infantiles_covid/files/comparaison_patho_moins_15.Rmd) 
- [Téléchargez l'article complet au format pdf](/articles/comparaison_pathologies_infantiles_covid/files/comparaison_patho_moins_15.pdf)

Nous comparons ici les taux d’hospitalisation brut défini comme étant le
rapport entre le nombre quotidien de passages aux urgences avec un
diagnostic médical posé par les urgentistes parmi l’ensemble des
passages aux urgences avec un diagnostic médical renseigné. Cette
proportion est exprimée pour 10 000 consultations.

Les données sont issues des du réseau “Oscour” de Santé publique France
disponibles sur l’interface Geodes
(<a href="https://geodes.santepubliquefrance.fr/" class="uri">https://geodes.santepubliquefrance.fr/</a>)
pour la tranche d’âge 0-14ans.

Pour chaque pathologie, nous sélectionnons dans l’interface le type de
pathologie, puis le taux d’hospitalisation hebdomadaire, les données
correspondant à la tranche d’âge 0-14 ans puis le format “données”.

Notre fichier de données est téléchargeable mais il est aussi possible d'extraire vos propres données depuis le site de Santé Publique France. 

Concernant les décès, nous donnons à titre de comparaison le nombre de
décès dû à la grippe par rapport à ceux du Covid19 pour les enfants de
moins de 15 ans dont ceux avec comorbidité associée.

## Comparaison des taux d’hospitalisation brut

**Nous pouvons constater que sur l’année 2020**

- les pathologies dûes à l’asthme sont restées sur un plateau très élévé
- les pathologies dûes aux pneumopathies et aux bronchites aigues ont atteint des niveaux très importants
- les hospitalisations dûes aux Covid19 sont sensiblement au même niveau que celle des gastro-enterites et sont largement en dessous de celles de l’asthme, des pneumopathies ou des bronchiolites.

## Comparaison des hospitalisations de l’année 2020 dûes aux pneumopathies par rapport aux autres années chez les enfants


### Comparaison avec les années précédentes

Nous pouvons constater que le nombre d’hospitalisation en 2020 dû à des
pneumopathies chez les enfants est largement au dessus des années
précédentes (Figure <a href="#fig:pneumo">5</a>).

La chute brutale des hospitalisations à partir de la semaine 17 peut
être expliquée par plusieurs hypothèses : abandon de soin (peur de la
population de se rendre à l’hôpital), réduction de la pollution et des
particules finies. Cette chute brutale (anormale sur la plan statistique
comparé aux années précédentes) se compense par la hausse des
hospitalisations observées au déconfinement (ce qui traduirait donc une
reprise en charge de ces pathologies non soignées au moment du
confinement).

Nous pouvons constater que par la suite les taux d’hospitalisation de
l’année 2020 se sont rapprochés des taux des années précédentes de la
semaine 30 à la semaine 36. Cependant, en semaine 36 on observe un
décrochage de la courbe avec une très nette augmentation de celle-ci et
créant un écart important avec les taux des années précédentes, qui
manifestement, ne se réduit pas à la fin de l’année 2020.


![Comparaison par année du taux d'hospitalisation dû aux pneumopathies chez les moins de 15 ans](/articles/comparaison_pathologies_infantiles_covid/img/pneumo_annee.png)
<p class="caption">
Figure 2: Comparaison par année du taux d’hospitalisation dû aux
pneumopathies chez les moins de 15 ans
</p>

### Comparaison par groupe d’âge

Nous comparons ici l’évolution du taux d’hospitalisation chez les
enfants par rapport à ceux des groupes d’âge 15-64 ans et ≥ 65 ans pour
l’année 2020 afin de constater l’écart de l’évolution de 2020 sur
l’ensemble des groupes d’âges.

Afin de tenir compte de l’écart d’amplitude de classes d’âge de chacun
des groupes d’âge, nous divisons par la population totale correspondant
à chaque groupe d’âge. Le calcul de ces populations de groupe d’âge est
issu des données des pyramides des âges au 1er janvier de chaque année
considérée et produites par l’Insee
(<a href="https://www.insee.fr/fr/statistiques/5007688?sommaire=5007726" class="uri">https://www.insee.fr/fr/statistiques/5007688?sommaire=5007726</a>)

<table>
<thead>
<tr class="header">
<th style="text-align: left;">Groupe d’âge</th>
<th style="text-align: left;">2020</th>
<th style="text-align: left;">2019</th>
<th style="text-align: left;">2018</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="text-align: left;">0-14 ans</td>
<td style="text-align: left;">12 032 908</td>
<td style="text-align: left;">12 707 443</td>
<td style="text-align: left;">12 172 566</td>
</tr>
<tr class="even">
<td style="text-align: left;">15-65 ans</td>
<td style="text-align: left;">41 520 403</td>
<td style="text-align: left;">41 588 985</td>
<td style="text-align: left;">41 652 795</td>
</tr>
<tr class="odd">
<td style="text-align: left;"><span class="math inline">≥</span> 65 ans</td>
<td style="text-align: left;">13 733 900</td>
<td style="text-align: left;">13 447 773</td>
<td style="text-align: left;">13 166 798</td>
</tr>
</tbody>
</table>

Nous constatons que cet écart du taux d’hospitalisation au regard des
années précédentes est le plus important chez les enfants que tous les
autres groupes d’âges (Figure <a href="#fig:comp1Pneumo">3</a>) avec
**34555 hospitalisations de plus au total sur l’année 2020** comparé à
la moyenne des 2 années précédentes, contre **7731 chez les 15-64 ans**
et **-5996 sur la tranche d’âge des plus de 64 ans** (solde négatif
traduisant que les périodes de hausses sont rattrapées par les périodes
de baisse de façon plus importante) en normalisant sur le nombre de
personnes du groupe d’âge 0-14 ans afin de tenir compte des disparité du
nombre de personnes dans chaque groupe d’âge.

Avec un ratio de 1 à 5 comparé au groupe d’âge des 0-64 ans (Figure
<a href="#fig:comp2Pneumo">4</a>) (pour le même nombre de personnes),
cette hausse très importante d’hospitalisations de pneumopathies chez
les enfants est absente les années précédentes (Figure
<a href="#fig:comp1Pneumo">3</a>).


![Comparaison par groupe d'âge du taux d'hospitalisation dû aux pneumopathies](/articles/comparaison_pathologies_infantiles_covid/img/pneumo_groupe_age.png)
<p class="caption">
Figure 3: Comparaison par groupe d’âge du taux d’hospitalisation dû aux
pneumopathies
</p>

![Nombre d'hospitalisation en plus pour la pneumoptahie par groupe d'âge](/articles/comparaison_pathologies_infantiles_covid/img/difference_pneumopathie_age.png)
<p class="caption">
Figure 4: Nombre d’hospitalisation en plus pour la pneumoptahie par
groupe d’âge
</p>

## Comparaison des hospitalisations de l’années 2020 dûes à la bronchite aigüe par rapport aux années précédentes chez les enfants

### Comparaison avec les années précédentes :


![Comparaison par année du taux d'hospitalisation dû aux bronchites aigües chez les moins de 15 ans](/articles/comparaison_pathologies_infantiles_covid/img/bronchite_annee.png)
<p class="caption">
Figure 5: Comparaison par année du taux d’hospitalisation dû aux
bronchites aigües chez les moins de 15 ans
</p>

### Comparaison par groupe d’âge

![Comparaison du taux d'hospitalisation dûe à la bronchite aigüe par groupe d'âge](/articles/comparaison_pathologies_infantiles_covid/img/bronchite_groupe_age.png)
<p class="caption">
Figure 6: Comparaison du taux d’hospitalisation dûe à la bronchite aigüe
par groupe d’âge
</p>

![Nombre d'hospitalisations en plus dû à la bronchite aigüe](/articles/comparaison_pathologies_infantiles_covid/img/difference_bronchite_age.png)
<p class="caption">
Figure 7: Nombre d’hospitalisations en plus dû à la bronchite aigüe
</p>

## Comparaison des hospitalisations de l’année 2020 dûes à l’asthme par rapport aux autres années chez les enfants


### Comparaison avec les années précédentes :

Les hospitalisations dûes à l’asthme chez les enfants de moins de 15 ans
sont très élevées au regard des années précédentes et restent sur un
haut plateau très peu descendant comparé aux autres années (Figure
<a href="#fig:athme">8</a>).

Tout comme pour les pneumopathies, on observe une baisse très nette des
taux d’hospitalisation durant la période de confinement et anormalement
basse par rapport aux années précédentes. L’augmentation visible à
partir de la semaine du déconfinement traduit une reprise en charge
hospitalière de ces pathologies non traitées durant la période de
confinement.

Cependant, comme pour les pneumopathies, on observe un écart très franc
entre les taux de l’année 2020 et ceux des années précédentes à partir
ici de la semaine 40 (Figure <a href="#fig:athmeComp1">9</a>) . Cet
écart se recreuse à partir de la semaine 45, semaine à laquelle
l’obligation du port du masque en milieu scolaire à partir de 6 ans a
été pratiquée. Comme nous pouvons le constater, cet écart ne se réduit
pas à la fin de l’année et reste constant sur l’ensemble de cette
période.

![Comparaison par année du taux d'hospitalisation dû à l'asthme chez les moins de 15 ans](/articles/comparaison_pathologies_infantiles_covid/img/asthme_annee2.png)
<p class="caption">
Figure 8: Comparaison par année du taux d’hospitalisation dû à l’asthme
chez les moins de 15 ans
</p>

### Comparaison par groupe d’âge

Cet écart est le plus grand parmi les autres groupes d’âge pour cette
même pathologie (Figures <a href="#fig:athmeComp1">9</a> et
<a href="#fig:asthmeComp2">10</a>) avec **5067 hospitalisations de plus
sur l’année 2020** comparé à la moyenne des 2 années précédentes, contre
**3514 chez les 15-64 ans** et **-7736 sur la tranche d’âge des plus de
64 ans en normalisant sur le nombre de personnes du groupe d’âge 0-14
ans**.

![Comparaison du taux d'hospitalisation par groupe d'âge](/articles/comparaison_pathologies_infantiles_covid/img/asthme_groupe_age.png)
<p class="caption">
Figure 9: Comparaison du taux d’hospitalisation par groupe d’âge
</p>

![Nombre d'hospitalisations en plus dû à l'asthme](/articles/comparaison_pathologies_infantiles_covid/img/difference_asthme_age.png)
<p class="caption">
Figure 10: Nombre d’hospitalisations en plus dû à l’asthme
</p>

## Le Covid est aussi virulent que la grippe chez les enfants : IL NE TUE PAS LES JEUNES !

### Considérations :

NON ! Le Covid19 ne tue pas les jeunes... Les jeunes ne sont jamais morts d'épidémie de grippe et ce n'est pas le Covid19 qui y changera quelque chose. Apprenons donc à relativiser, à souffler, à revenir à la raison. Chaque parent a peur pour son enfant et c'est légitime. Mais Le Covid ne TUE PAS LES JEUNES !

Et pour s'en convaincre, rien de tel que de regarder les chiffres qui parlent d'eux-même !

**Concernant la grippe :**
Santé publique France mentionne que :
- **12 décès en 2020** dû à la grippe ont été rapportés parmi les mineurs dont **7 avec une ou plusieurs comorbidités** \[1\]
- **8 décès en 2019** dû à la grippe sont survenus parmi les mineurs dont 4 sans facteur de risque, **3 avec une ou plusieurs comorbidités** et 1 sans information disponible \[2\]
- **10 décès sont survenus en 2018** parmi les mineurs dont **6 avec un facteur de risque**, 3 sans facteur de risque et 1 sans information disponible \[3\]
- **13 décès** dûs à la grippe sont survenus en 2016 et **36 décès** en 2015 \[4\].

**Concernant la covid19 :**
- Au 31/12/2020, 4 décès dû à la covid19 sont rapportés chez les 0-9 ans et 6 décès pour les 10-18 ans (soit **10 au total**) \[5\] dont **3 avec comorbodité** \[6\].

Donc souffons un peu, respirons à plein poumon, repensons à des choses positives et sortons de cette peur ambiante que les médias alimentent matin, midi et soir, dimanche et jour férié compris...

## Conclusions

On peut constater que le Covid19 n'entraîne pas une hausse des 
hospitalisations ni des décès chez les enfants, les niveaux de ces
indicateurs étant similaires à ceux de la grippe et de la
gastro-entérites dans ces classes d'âge.

En revanche, les hospitalisations dûes aux pneumopathies et à
l'asthme sont nettement en très forte hausse comparé aux années
précédentes. Les écarts créés par l'augmentation des
hospitalisations de ces pathologies correspondent aux dates d'entrée
en rigueur des mesures sanitaires notamment en milieu scolaire avec
**34555 hospitalisations de plus pour les pneumopathies** comparé à la moyenne des deux années précedentes et **5067 hospitalisations pour l'asthme**, 
**soit 39622 hospitalisations et comptabilisées seulement sur ces deux pathologies** (contre 30291 pour les 15-64 ans et -14580 pour les plus de 64 ans).

Ces hausses sont-elles dûes à l'obligation du port du masque chez nos enfants ? La question se pose. Etant donné qu'aucune étude d'impact du port du masque chez des enfants, notamment chez les plus jeunes, n'a jamais été menée (rappellons qu'un enfant de primaire court, joue au ballon, le temps des récréations avec son petit masque bien posé sur le nez pour éviter les brimades, ce qui n'a strictement rien n'à voir avec le contexte dans lequel les soignants portent un masque), cette question de santé publique aurait dû être abordée et éclaircie avant que cette mesure soit prise. Mais cela aurait demandé de la compétence et de la responsabilité, voir même un soupçon de mâturité de la part de notre gouvernement. Bref, autant rêver !

## Références

 1. France S publique. Bulletin épidémiologique grippe, semaine 12.
Saison 2018-2019. 2020. <https://www.santepubliquefrance.fr/maladies-et-traumatismes/maladies-et-infections-respiratoires/grippe/documents/bulletin-national/bulletin-epidemiologique-grippe.-bilan-de-la-surveillance-saison-2019-2020>.

 2. France S publique. Bulletin épidémiologique grippe, semaine 12.
Saison 2018-2019. 2019.
<https://www.santepubliquefrance.fr/maladies-et-traumatismes/maladies-et-infections-respiratoires/grippe/documents/article/surveillance-de-la-grippe-en-france-saison-2018-2019>.

 3. France S publique. Bulletin épidémiologique grippe, semaine 12.
Saison 2017-2018. 2018.
<https://www.santepubliquefrance.fr/maladies-et-traumatismes/maladies-et-infections-respiratoires/grippe/documents/article/surveillance-de-la-grippe-en-france-saison-2017-2018>.

 4. France S publique. Grippe - caractéristiques des hospitalisations
avec diagnostic en france de 2012 à 2017.
<https://www.santepubliquefrance.fr/les-actualites/2019/grippe-caracteristiques-des-hospitalisations-avec-diagnostic-en-france-de-2012-a-2017>.

 5. <https://www.data.gouv.fr/fr/datasets/r/08c18e08-6780-452d-9b8c-ae244ad529b3>.

 6. France S publique. COVID-19 : Point épidémiologique du 14 janvier
2021. <https://www.santepubliquefrance.fr/maladies-et-traumatismes/maladies-et-infections-respiratoires/infection-a-coronavirus/documents/bulletin-national/covid-19-point-epidemiologique-du-14-janvier-2021>.
