---
title: Gérer son patrimoine commence par un grand inventaire
summary: De l'importance de correctement inventorier sa richesse, sans oublier sa première composante ...
date: "2020-07-19"

math: true
reading_time: true  # Show estimated reading time?
share: true  # Show social sharing links?
profile: true  # Show author profile?
comments: true  # Show comments?
draft: false

# Optional header image (relative to `static/img/` folder).
header:
  caption: ""
  image: ""
---

##  La première étape d'un bilan financier est la simulation de son patrimoine. L'objectif est d'embrasser une vue large de ses ressources, actuelles mais aussi à venir.

### Qu'est-ce qu'une simulation de l'épargne?

La simulation d'épargne consiste à projeter le capital détenu d'une personne ou d'un ménage jusqu'à une échéance choisie, sous une hypothèse de rendement, et en ajoutant chaque année future l'épargne de la période. Il existe un grand nombre de simulateurs en ligne comme  celui de [Cardif](https://www.cardif.fr/placement-epargne/simulation-epargne), ou celui du [Crédit Mutuel](https://www.creditmutuel.fr/fr/simulations/epargne.html). La plupart des simulateurs ont pour objectif d'évaluer la capacité de l'épargnant à réaliser un projet précis ou sont attachés à un produit d'épargne particulier, comme un contrat d'assurance vie. Notre objectif étant de simuler le patrimoine global de l'épargnant en adoptant une perspective de cycle de vie, nous ne distinguons pas différents projets ou produits d'épargne.

### Simuler la patrimoine

Commençons par poser quelques notations :
+ $w_0$ est le patrimoine de l'épargnant au moment de la simulation
+ $r$ est le rendement annuel prévu de l'épargne
+  $s_t$ est la capacité d'épargne l'année $t$
+  $p$ est le taux de progression annuel de l'épargne
+ $T$ est la durée du placement exprimée en années

Le patrimoine couvre l'ensemble des composantes de la richesse : livrets et comptes bancaires, épargne retraite, contrats d'assurance vie, immobilier (valeur de marché nette de l'endettement résiduel), compte titres, ...
Le rendement annuel prévu est une moyenne pondérée des rendements prévus sur les différentes catégories du patrimoine. Le rendement de la propriété de la résidence principale est la somme annuelle des loyers économisés si l'épargnant était locataire, après déduction des intérêts restant dus sur le crédit immobilier, des travaux immobiliers et de la fiscalité sur les biens immobiliers (taxes d'habitation et foncière).
La capacité annuelle d'épargne est la différence entre les revenus annuels nets de toute fiscalité (cotisations sociales, impôt sur le revenu, ...) et les dépenses annuelles.
La durée de placement doit être suffisamment longue. La date terminale $T$ peut correspondre au pic de patrimoine, le moment où les dépenses d'épargne le revenu, qui peut être la date de départ à la retraite ou au-delà si l'épargnant prévoit de continuer à épargner après la retraite.

<a name="eq1"></a>
Commençons par nous placer dans $T$ années et notons $w_T$ le patrimoine final issu de l'accumulation de l'épargne et la capitalisation des intérêts :
$$
w_T = (1+r)^T w_0 + (1+r)^{T-1} s_1 \\ + (1+r)^{T-2} s_2 + ... + (1+r) s_{T-1} + s_T
$$

Prenons l'exemple d'un épargnant âgé de 35 ans disposant d'un patrimoine de 30 000 euros et dont les revenus annuels sont de 36000 euros nets. Après soustraction de ses dépenses, sa capacité d'épargne annuelle est de 11 000 euros. Le rendement de son épargne est estimé à 1% et la progression annuelle de son épargne à 1 %. Son horizon de placement est de 30 ans. A l'aide de ces données, nous pouvons calculer une richesse terminale $w_T$ d'environ 485 000 euros. Ce sont des montants conséquents qui, bien qu'incertains car fondés sur des hypothèses, donne une bonne idée du défi attendant l'épargnant tout au long de sa vie active en termes de choix de placement.

### Simuler le patrimoine actuel et futur

Une perspective encore plus instructive consiste à évaluer sa richesse totale non pas dans 35 ans mais *dès aujourd'hui* grâce à la méthode d'actualisation des flux. L'actualisation est l'opération inverse de la capitalisation des flux financiers. Un euro placé pendant deux ans au taux d'intérêt $r$ permet d'obtenir $(1+r)^2$ euros. Inversement, si nous retournons la flèche du temps, $(1+r)^2$ euros disponibles dans deux ans sont équivalents à 1 euros aujourd'hui. Ou 1 euro dans deux ans est équivalent à $(1+r)^{-2}$ euros aujourd'hui. Les deux opérations sont symétriques et représentés dans la Figure 1.

Figure 1 Capitalisation et actualisation d'un euro sur deux périodes
![actualisation des flux](http://gdre.leo-univ-orleans.fr/direr/blog/actualisation.png)
<a name="eq2"></a>
Actualisons de la richesse accumulée en 30 ans à la date d'aujourd'hui : $W_0 = (1+r)^{-T}w_T$. Cela revient à appliquer l'opération d'actualisation à l'ensemble des flux d'épargne de [l'équation d'accumulation](#eq1) :
$$
W_0= w_0 + (1+r)^{-1} s_1 + (1+r)^{-2} s_2 + ... + (1+r)^{-T} s_T 
$$

L'épargnant détient des "droits" sur deux catégories très différentes de  sa richesse : la richesse acquise $w_0$ et la richesse potentielle $h$ qu'il projette d'obtenir sur la base de de ses revenus à venir. Les deux composantes forment  la richesses inter-temporelle. Si nous reprenons l'exemple numérique précédent, nous obtenons $W_0$ = 360 000 euros, qui se décompose en $w_0$ = 30 000 euros de richesse acquise et $h$ = 330 000 euros de richesse future.

La richesse intertemporelle est principalement composée de richesse à venir dans la première période de cycle de vie. Dans l'exemple, elle représente 92 % de la richesse totale. Mais, puisque cette composante de la richesse n'est pas à strictement parlé détenu par l'épargnant, quel est son intérêt ? L'intérêt de la prendre en compte dans la gestion de son patrimoine est multiple.

Premièrement, elle permet d'adopter une perspective longue d'accumulation du patrimoine, de manipuler des ordres de grandeur pertinents et de planifier son épargne et sa richesse. Un épargnant qui prend des décisions d'allocation sur la seule base de son patrimoine existant prend le risque d'une gestion à courte vue, faute d'anticiper l'évolution de son patrimoine.

Deuxièmement, la richesse future n'est pas qu'une simple référence hypothétique. Elle peut être partiellement convertie en liquide pour acquérir des biens durables. Reprenons notre exemple et supposons que notre épargnant désire s'endetter pour acheter sa résidence principale. Combien peut-il prétendre emprunter ? La banque lui accordera, après étude de sa capacité d'épargne, un montant déterminée de façon proche de la méthode de calcul de sa [richesse potentielle](#eq2). Sur les 330 000 euros qu'il peut dégager dans le futur, la banque lui accordera éventuellement 200 000 euros sur 20 ans. Cet écart s'explique par un comportement prudent de la banque et par un changement de deux paramètres dans le calcul de $h$ : la richesse potentielle de l'emprunteur sur 20 ans est plus faible que sur 30 ans et le taux qui actualise l'épargne future est le taux du crédit. Sur 20 ans et un taux débiteur de 2 %, nous obtenons $h$ = 229 000 euros.

Enfin, la richesse potentielle est une référence importante pour une bonne allocation de son patrimoine, comme nous le verrons dans le post suivant.

### Comment évolue la composition de la richesse au cours du cycle de vie ?

Pour le voir, faisons un saut dans le temps d'une année pleine. A ce moment-là, l'épargnant a épargné et accumulé de la richesse supplémentaire. mais dans le même temps, il dispose d'une année en moins d'épargne entrant dans la formule de la richesse potentielle :
$$
W_1 = (1+r) w_0 + s_1 + (1+r)^{-1} s_2 + (1+r)^{-2} s_3 \\ + ... + (1+r)^{-(T-1)} s_T 
$$

Un fraction de la richesse potentielle $h$ est converti en richesse acquise. Encore une année plus tard, sa richesse intertemporelle est :
$$
W_2 = (1+r)^2 w_0 + (1+r) s_1 + s_2 + (1+r)^{-1} s_3  \\ + ... + (1+r)^{-(T-2)} s_T 
$$

A la fin de sa période d'accumulation, sa richesse intertemporelle est composée en totalité de sa richesse acquise et nous retrouvons la formule de la [richesse capitalisée](#eq1).

Si nous reprenons notre exemple numérique, la figure 2 indique comment évolue la richesse et ses deux composantes sur le cycle de vie de l'épargnant.

Figure 2 Évolution de la richesse et de sa composition sur le cycle de vie

![évolution de la composition du patrimoine](http://gdre.leo-univ-orleans.fr/direr/blog/composition.png)
En début de cycle de vie, l'épargnant dispose essentiellement d'une richesse potentielle qu'il convertit progressivement en richesse acquise. La richesse intertemporelle et la richesse acquise augmente de façon légèrement exponentielle avec la capitalisation des intérêts de 1 %. Même un un rendement de 1 % sur le patrimoine est important une fois capitalisée sur 30 ans. La richesse finale ne serait que de 416 500 euros avec un rendement nul au lieu de 485 000 euros.
