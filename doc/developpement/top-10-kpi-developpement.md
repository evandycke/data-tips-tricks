# Top 10 des indicateurs d'une équipe de développement

## Cycle Time

### Qu'est-ce que c'est ?

Le Cycle Time est le temps nécessaire pour effectuer une tâche donnée, telle que la correction d'un bogue ou l'ajout d'un nouveau code.

### Pourquoi est-ce important ?

Le Cycle Time est une mesure d'ingénierie clé pour acquérir une meilleure compréhension de vos processus de travail. Vous pouvez utiliser le Cycle Time pour identifier le type de travail qui prend particulièrement de temps à réaliser, ce qui vous permet de localiser les goulots d'étranglement qui ralentissent vos projets. Cette métrique est également précieuse car elle vous aide à estimer la durée de vos projets futurs.

### Comment le calculer ?

```
Date de fin du projet - Date de début du projet
```

Le Cycle Time est le temps qui s'écoule entre le moment où une tâche entre dans la phase "en cours" et le moment où elle est considérée comme terminée. La façon évidente de mesurer le Cycle Time d'une tâche est de compter le nombre de jours passés à travailler sur cette tâche.

Cependant, il y a encore un débat dans de nombreuses organisations sur la question de savoir si le Cycle Time devrait inclure les heures non travaillées ou non. La meilleure façon de trancher le débat est de regarder les choses du point de vue de l'expérience client. Disons que vous mesurez le Cycle Time en excluant les heures chômées et les week-ends. Sur la base des données historiques, vous prédisez que votre Cycle Time est de 8 jours et l'annoncez à vos clients. Vos clients attendent (à juste titre) un livrable dans exactement huit jours. Cependant, vous ne pourrez livrer le produit qu'en 15 jours car vous avez exclu les heures chômées et les week-ends de vos calculs. Du point de vue de vos clients, vous serez en retard. L'exclusion des heures non travaillées peut améliorer l'apparence de votre Cycle Time en interne, mais cela entraînera certainement l'insatisfaction des clients. Je vous laisse deviner lequel est le plus important.

### À quoi ressemble-t-il ?

Il est intéressant d'afficher le temps de cycle sous forme de graphique montrant son évolution et le type de tâche. Cela vous permet de remarquer si votre temps de cycle change avec le temps ou en fonction du type de tâche dont il s'agit.

## Mean Time To Repair (MTTR)

### Qu'est-ce que c'est ?

En tant que mesure de production, MTTR fait référence au temps nécessaire aux ingénieurs pour réparer un problème logiciel. En tant que mesure de sécurité, il fait référence au temps nécessaire aux ingénieurs pour déployer une solution à partir du moment où ils découvrent une faille de sécurité.

### Pourquoi est-ce important ?

Le MTTR commence au moment où une défaillance est détectée et englobe le temps de diagnostic, le temps de réparation, les tests et toutes les autres activités jusqu'à ce que le service soit retourné aux utilisateurs finaux. Cette métrique montre les performances du logiciel en production. Les pannes logicielles sont inévitables, il est donc important de mesurer la rapidité avec laquelle il récupère. Cette métrique est précieuse car elle montre combien de temps les utilisateurs doivent attendre avant de pouvoir réutiliser le logiciel. C'est ce que beaucoup d'utilisateurs perçoivent comme un support technique. Cette mesure a un impact sur l'expérience client, c'est pourquoi il est essentiel de la mesurer. Garder ce nombre bas vous aide à maintenir un niveau élevé pour votre produit.

### Comment le calculer ?

```
Temps d'arrêt total / Nombre total de défaillance
```

Le MTTR est calculé en divisant le temps d'arrêt total causé par les défaillances par le nombre total de défaillances.

Par exemple, si un système tombe en panne trois fois par mois et que les défaillances entraînent un total de six heures d'indisponibilité, le MTTR serait de deux heures. MTTR = 6 heures / 3 échecs = 2 heures

Lorsque cette valeur diminue au fil du temps, cela signifie que les développeurs deviennent plus efficaces pour comprendre et corriger les bogues.

### À quoi ressemble-t-il ?

Il est important d'afficher un MTTR afin de voir son évolution. En fait, voir comment cette métrique évolue vous permet de comprendre si votre équipe résout les problèmes plus rapidement et de manière plus efficace. Si cette métrique ne diminue pas, quelque chose est anormal. Les problèmes sont souvent redondants. Si votre équipe d'ingénieurs ne résout pas les problèmes plus rapidement, il peut être nécessaire de comprendre la cause première des problèmes au lieu d'utiliser des solutions rapides.

## Mean Time Between Failures (MTBF)

### Qu'est-ce que c'est ?

Le temps moyen entre pannes ou MTBF fait référence au temps moyen entre les pannes du système.

### Pourquoi est-ce important ?

Le MTBF est une mesure de maintenance utilisée pour évaluer la fiabilité et la disponibilité d'un système. Dans le cas d'un logiciel, par exemple, il indique combien de temps il peut fonctionner sans panne. Il est important de surveiller le MTBF car avoir un MTBF très faible signifie que le système nécessite beaucoup de maintenance et d'améliorations. De plus, avoir trop de pannes peut entraîner une perte d'utilisateurs / clients. Par conséquent, mesurer le MTBF est un moyen de mieux connaître et d'améliorer la qualité de votre produit. En fait, le MTBF peut être utilisé pour optimiser le calendrier de maintenance prédictive, évitant ainsi les défaillances du système.

### Comment le calculer ?

```
Temps total de disponibilité du système / Nombre de pannes sur la même période
```

Par exemple, si votre site Web était opérationnel pendant une journée entière avec deux pannes qui prenaient chacune une heure à réparer, votre MTBF serait de 11 heures.

MTBF = 22 heures / 2 échecs.

Plus le MTBF est élevé, plus notre système est fiable et disponible. Lorsque vous examinez le MTBF, vous ne devez pas prendre en compte les temps d'arrêt dus à la maintenance ou à la mise à jour prévue. Au lieu de cela, nous voulons nous concentrer sur des problèmes inattendus.

### À quoi ressemble-t-il ?

Cette mesure doit être affichée sur un graphique linéaire. L'axe des Y doit représenter le MTBF et l'axe des X doit représenter le temps avec différentes granularités (heures, jours, mois) selon le produit. L'objectif est de maintenir un MTBF aussi élevé que possible car cela se traduit par très peu de défaillances inattendues.

## Change Failure Rate (CFR)

### Qu'est-ce que c'est ?

Le taux d'échec des modifications ou CFR représente la proportion de déploiements ayant échoué par rapport au nombre total de déploiements. Dans cette métrique, nous ne prenons pas en compte les erreurs qui ont été commises lors du développement ou des tests ou les problèmes qui surviennent après une longue période de temps. Nous nous concentrons uniquement sur les erreurs qui ont été commises en raison d'une modification du système, telles que de nouvelles fonctionnalités ou des solutions rapides.

### Pourquoi est-ce important ?

Il est intéressant d'examiner le CFR car c'est un bon indicateur de la qualité des changements qui sont déployés. En fait, si le CFR est trop élevé, cela signifie que vous pouvez avoir des problèmes de test ou de revue du code avant le déploiement. D'autre part, un bon CFR signifie que votre équipe est en mesure d'identifier les problèmes avant le déploiement et que vous n'avez pas à perdre de temps à les résoudre par la suite.

### Comment le calculer ?

```
Nombre d'échec de déploiement / Nombre de déploiements
```

Si votre équipe a effectué 20 déploiements au cours de la semaine et que 4 d'entre eux ont entraîné des problèmes qui ont dû être résolus immédiatement après le déploiement, le CFR de votre équipe est de 20%.

### À quoi ressemble-t-il ?

Il est intéressant d'examiner l'évolution de cette métrique au fil du temps. Par conséquent, l'affichage du CFR sur l'axe Y d'un graphique linéaire avec le temps (jours/semaines/mois) sur l'axe des X vous permettra de regarder facilement les performances de votre équipe. L'objectif de votre équipe est de réduire cette métrique autant que possible. Même s'il serait impossible d'avoir un CFR de 0%, les équipes d'ingénieurs hautement performantes devraient avoir un CFR inférieur à 15%.

## Change Lead Time (CLT)

### Qu'est-ce que c'est ?

Le Change Lead Time (ou CLT) est une mesure essentielle qui évalue la vitesse de déploiement d'une équipe. Il représente la durée moyenne d'implémentation, de test et de livraison d'un morceau de code.

### Pourquoi est-ce important ?

Le CLT est l'un des KPI les plus importants à suivre lors de l'évaluation de l'efficacité de votre équipe dans le processus de développement. Si votre délai de changement est très long, il peut être intéressant d'examiner la chaîne de développement pour voir où il y a un problème. Par exemple, il pourrait y avoir un goulot d'étranglement dans le processus si une personne le long de la chaîne est surchargée de tâches. D'autre part, un délai de changement court est un signe de flexibilité et de réactivité aux problèmes.

### Comment le calculer ?

```
Somme de (Date de fin de changement - Date de début de changement) / Nombre de changements
```


Cette semaine, votre équipe a apporté 2 modifications à votre produit qui ont pris respectivement 2 et 4 jours entre leur validation et leur déploiement. Le délai de changement est de 3 jours.

### À quoi ressemble-t-il ?

L'évolution de votre CLT peut être surveillée à l'aide d'un graphique linéaire. L'idée est qu'en gardant un délai de changement faible, vous vous assurez que les changements que vous apportez à votre produit sont effectués efficacement et que vous êtes plus flexible.

## Test Coverage Ratio (TCR)

### Qu'est-ce que c'est ?

La couverture des tests fait référence à la proportion de votre code qui est exécutée lors de l'exécution de votre suite de tests.

### Pourquoi est-ce important ?

En prenant en compte une métrique de couverture de test, vous êtes en mesure de mieux identifier les écarts entre les exigences et les tests. Par conséquent, vous pouvez facilement découvrir des zones de votre code qui ne sont pas testées. De plus, la couverture de test peut indiquer que vous devez créer plus de cas de test pour une meilleure couverture, mais elle peut également aider à identifier et à éliminer les cas de test qui ne sont pas nécessaires. Dans l'ensemble, avoir une métrique de couverture de test vous aidera à avoir plus de contrôle sur vos tests, rendant ainsi le cycle de test plus fluide et de meilleure qualité.

### Comment le calculer ?

```
Nombre de lignes testées / Nombre de lignes total
```

Il est considéré comme adéquat que votre suite de tests couvre au moins 80% de votre code. En fait, plus la couverture est bonne, plus vous aurez de chances de découvrir des zones qui doivent être corrigées. Même si nous aimerions que la couverture de test soit aussi élevée que possible, vous ne devriez pas vous concentrer sur l'atteinte d'une couverture de 100% en écrivant des scripts de test vagues, mais davantage sur les exigences de votre logiciel.

### À quoi ressemble-t-il ?

Le TCR doit être affiché sur un graphique pour pouvoir voir comment il évolue dans le temps. Par exemple, si vous constatez une baisse du taux de couverture des tests après avoir apporté des mises à jour à votre code, cela peut être dû au fait que vous oubliez d'écrire des tests qui exécutent certaines parties du nouveau code.

## Release Burndown

### Qu'est-ce que c'est ?

Le Release Burndown est une métrique utilisée en particulier dans les projets Scrum poursuivre l'avancement d'un projet en examinant la quantité de travail restante.

### Pourquoi est-ce important ?

L'une des principales utilisations du Release Burndown est de permettre aux équipes de surveiller leurs progrès. Cependant, il peut également être utilisé pour fixer des objectifs et motiver l'équipe à les atteindre. De plus, regarder le tableau Release Burndown de votre équipe vous aidera également à voir si votre projet est à l'heure ou s'il y a des problèmes qui ont conduit à un ralentissement.

### Comment le calculer ?

```
Quantité de travail qu'il reste à faire
```

Le Release Burndown peut être exprimé en termes d'unités différentes telles que le nombre d'heures de travail restantes. Dans le développement de logiciels, les équipes aiment également utiliser le nombre d'exigences qui doivent encore être traitées pour l'application. Vous devez adapter l'unité de cette métrique à votre projet afin qu'elle soit aussi facilement compréhensible que possible par les membres de votre équipe.

### À quoi ressemble-t-il ?

Le graphique Release Burndown peut être un graphique à barres ou un graphique linéaire avec les unités de travail restant sur l'axe des Y et certaines périodes sur l'axe des X. Ce tableau devrait être mis à jour à chaque période (p. ex. chaque semaine), avec la quantité de travail qui a été effectuée et la projection des travaux à effectuer pour les périodes suivantes jusqu'à la fin du projet.

## Deployment Frequency

### Qu'est-ce que c'est ?

La fréquence de déploiement fait référence au nombre de déploiements effectués sur votre projet au cours d'une période de temps définie. S'il est mieux adapté à votre projet, vous pouvez également compter le nombre de fonctionnalités ajoutées à la place des déploiements.

### Pourquoi est-ce important ?

L'examen de la fréquence de déploiement d'un projet vous permet de surveiller la vitesse de votre projet. D'une part, si votre fréquence de déploiement est trop faible, cela peut indiquer que vous rencontrez des problèmes avec l'un des déploiements ou que vous avez un goulot d'étranglement qui ralentit votre processus de développement. D'autre part, avoir une fréquence de déploiement excessivement élevée peut également signifier que certaines fonctionnalités sont déployées trop rapidement sans suffisamment de tests ou de révisions, ce qui peut entraîner des défaillances du système.

### Comment le calculer ?

```
Nombre de déploiements / (Date de fin - Date de début)
```

Votre équipe a déployé 21 nouvelles fonctionnalités au cours des deux dernières semaines. Par conséquent, la fréquence de déploiement de votre équipe est de 1,5 déploiement par jour.

### À quoi ressemble-t-il ?

Il peut être intéressant d'examiner l'évolution de la fréquence de déploiement au fil du temps. En affichant sur l'axe Y d'un graphique linéaire la fréquence de déploiement avec le temps (jours/semaines/mois) sur l'axe X, vous serez en mesure d'évaluer très facilement la vitesse de développement de votre équipe.

## Pull Request Flow Ratio

### Qu'est-ce que c'est ?

Ler atio de flux de Pull Request (PR) fait référence à la somme des PR ouvertes sur la somme des PR fermées sur la même période.

### Pourquoi est-ce important ?

L'examen de ce ratio peut vous donner des informations importantes sur l'équilibre entre les fonctionnalités en cours de développement et celles qui sont déployées. Vous devez avoir autant de PR ouvertes que de PR fermées. En fait, avoir un ratio déséquilibré peut signifier que vous avez trop de PR ouvertes et qu'elles font la queue pour être déployées. Cela peut également être un signe que le délai d'exécution de la PR ouverte et que vous devez résoudre ce problème. Dans l'ensemble, il est préférable d'avoir un ratio de 1-1 pour vous assurer que votre processus est fluide et prévisible.

### Comment le calculer ?

```
Nombre de PR ouvertes / Nombre de PR fermées
```

Cette semaine, vous avez eu 10 PR ouvertes alors que seulement 6 PR fermées. Le rapport est donc de 5/3. Il serait intéressant d'examiner le processus des PR ouvertes pour voir si nous pouvons réduire leur délai et améliorer l'efficacité de notre processus de développement.

### À quoi ressemble-t-il ?

Il est préférable de surveiller le ratio de flux de PR au fil du temps, car l'objectif est de viser un ratio de 1-1. En l'affichant sur l'axe Y d'un graphique linéaire de ce KPI avec le temps (jours/semaines/mois) sur l'axe X, vous serez en mesure d'évaluer l'équilibre entre le travail mis en place pour développer certaines fonctionnalités et celles qui sont déployées.

## Code Churn Rate (CCR)

### Qu'est-ce que c'est ?

Le taux de désabonnement du code mesure le nombre de fois qu'un morceau de code est modifié au cours d'une période donnée.

### Pourquoi est-ce important ?

Le CCR est essentiel car il aide à évaluer votre processus de développement. L'objectif principal du CCR est d'évaluer la qualité de votre code. En règle générale, plus vous apportez de modifications à votre code, plus vous risquez de faire des erreurs. Un CCR élevé peut être un signe qu'il y a trop de remaniement sur votre projet. Ce remaniement peut être causé par des problèmes tels qu'une mauvaise communication des objectifs du projet ou un manque de compétences en codage. De plus, regarder cette métrique vous permet d'identifier les parties de votre code qui doivent être testées ainsi que la répartition de vos ressources entre les différents modules de votre projet.

### Comment le calculer ?

```
(Lignes ajoutées + lignes supprimées + lignes modifiées) / Total de lignes
```

Disons que vous avez un script de 1000 lignes au total. Vous modifiez 100 lignes, ajoutez 200 lignes et supprimez 75 lignes, vous avez alors un CCR de 37,5%. Une mauvaise compréhension des exigences de vos clients pourrait en être la cause et l'amélioration de la communication avec eux pourrait aider à améliorer l'efficacité du projet.

### À quoi ressemble-t-il ?

Le CCR est généralement surveillé pendant de courtes périodes, telles que des semaines. Regarder l'évolution hebdomadaire de cette métrique vous permettra de détecter des améliorations ou des problèmes dans le développement de votre code. On dit souvent qu'il est préférable d'avoir un faible CCR. Cependant, il est impossible d'atteindre un CCR car vous devez toujours modifier votre code indépendamment de vos compétences en codage. En fait, avoir un CCR trop faible peut signifier que vous vous concentrez trop sur la vitesse et non sur la qualité du code. Plus généralement, il est préférable d'avoir un CCR compris entre 10% et 30%.

## On pourrait également encore ajouter ...

1. Nombre de bugs identifiés
2. Répartition des bugs par module (W-1 vs W)
3. Score de qualité hebdomadaire vs objectif
4. Indicateurs et temps forts de la semaine
* Taux de disponibilité
* Temps en mode dégradé
5. Statistiques d'intégration continue
6. Livraison de la semaine
7. Incidents de la semaine