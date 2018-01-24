# Comment contribuer

:+1::tada: Premièrement, merci de prendre de votre temps pour contribuer! :tada::+1:

Tout le monde est susceptible d'aider. voici comment faire grandir ce projet :

* Fourcher le dépot / (Fork It)
* Apporter vos évolutions et/ou correction
* Envoyer une pull request

Votre travail sera alors pris en compte dés que possible (des suggestions sur le changement, améliorations  peuvent être faite)

N'oubliez pas d'ajouter des tests, assurez vous que tout les tests soit passant, merci de respecter les standards de codes du projet.

Une fois le dépôt fourché, vous pouvez suivre les changement du dépôt principal (upstream) en utilisant cette commande.

```
git remote add upstream https://github.com/tisseurdetoile/pub.git
```

vous pouvez alors créer vos propre branches, en suivant cette nomenclature :

```
git checkout -b <prefix>/<micro-titre>-<numéro-de-issue>
```

Une fois vos changement finit (git commit -am '<message-de-description>'), récupération des changements amonts:

```
git checkout master
git pull --rebase origin master
git pull --rebase upstream master
git checkout <votre-branche>
git rebase master
```

Pour finir, publiez vos changements:

```
git push -f origin <votre-branche>
```

Vous devriez être capable de faire une pull request.

Les Commit messages

Merci de nettoyer votre histoire git avant de pousser.

Les messages Git devraient toujours avoir un micro-titre comme une balise, écrite en CamelCase. Le message lui-même devrait commencer par un verbe écrit au passé et devrait décrire une action. Les commits devraient être atomiques (une action = un commit).

Par exemple, la branche fix/total_negatif-6 pourrait avoir un commit [NegativeTotal] La valeur doit être absolue.

