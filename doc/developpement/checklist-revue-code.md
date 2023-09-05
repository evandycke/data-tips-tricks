# Check-list d'une revue de code

## Portée

* [ ] La story est prioritaire
* [ ] La story est petite
* [ ] La story minimise le fluage
* [ ] Aucun changement parasite
* [ ] Modifications hors tâche ajoutées au backlog

## Fonctionnement

* [ ] La spécification est correcte et complète
* [ ] La mise en oeuvre suit les spécifications
* [ ] Plan de test créé
* [ ] Tests unitaires créés et/ou mis à jour
* [ ] Branche fusionnée dans la branche Master
* [ ] Toutes les modifications testées
* [ ] Cas marginaux couverts
* [ ] Impossible de trouver un moyen de casser le code
* [ ] Impossible de trouver comment ces changements cassent une autre partie du système
* [ ] Toutes les tâches "terminées"
* [ ] ZÉRO DÉFAUT CONNU

## Défense

* [ ] Toutes les entrées des méthodes publiques validées
* [ ] Échoue bruyamment s'il est mal utilisé
* [ ] Tous les codes de retour cochés
* [ ] Sécurité
* [ ] Nous avons nettoyé toutes les ressources temporaires créées
* [ ] Les fichiers d'entrée sont archivés

## Facile à lire et à comprendre

* [ ] Abstraction appropriée et décomposition du problème
* [ ] Interface minimale exposée
* [ ] Cacher des informations
* [ ] Principe commande-requête
* [ ] Bonne dénomination
* [ ] Documentation et commentaires significatifs
* [ ] Entièrement refactorisé (utiliser un jugement avec le code existant)

## Style et mise en page

* [ ] Toutes les inspections sont réussies
* [ ] Exécution du formateur de code
* [ ] Pas de style de code malodorant
* [ ] Longueur de ligne, style conforme aux directives du projet

## Considérations finales

* [ ] VOUS COMPRENEZ PLEINEMENT LE CODE ET L'IMPACT DES CHANGEMENTS QUE VOUS AVEZ APPORTÉS ET IL... est incassable, est réellement fait, passera l'examen du code, vous rendrait fier de présenter vos changements à d'autres programmeurs en public, c'est facile à réviser, branche correcte, pas de code parasite, modifications de schéma documentées, branche fusionnée dans la branche maître, réussite des tests unitaires, plan de test manuel terminé et exécuté, toutes les modifications validées et poussées, demande d'extraction créée et révisée, Jira mis à jour