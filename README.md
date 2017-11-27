# TestGithub

How to use git !

## Table des matières

1. [Branch](#branch)
2. [Commit](#commit)
3. [Merge](#merge)
4. [Helpfull link](#helpfull-link)


## Branch
Créer une nouvelle branche :
```sh
$ git checkout -b newBranch
```

Positionner le HEAD sur une branche :
```sh
$ git checkout newBranch
```

Voir toute les branche sur origine + local :
```sh
$ git branch -a
```

Mise à jour des branches depuis origine :
```sh
$ git fetch --all
```

Suppression d'une branche et push vers origin:
```sh
$ git branch -d fb-branch
$ git push origin :fb-branch
```


## Commit
Ajouter les modifications au commit :
```sh
$ git add .
```

Créer un commit avec commentaire :
```sh
$ git commit -m "Commit test"
```

## Merge

Merge une branche sur la branche actuel avec ses historiques de commit :
```sh
$ git merge  branchToMerge
```

Merge une branche sur la branche actuel sans ses historiques de commit :
```sh
$ git merge --no-ff branchToMerge
```

Mise à jours de la branche actuel par rapport à une autres :
```sh
$ git rebase origin/branchSource
```

## Other

Rajouté un remote et push une branch :
```sh
$ git remote add <remote-alias> <url>
$ git push <remote-alias> <branch>
```

Annulé un commit sur une branch(ex: develop) et changer ce commit de branch :
```sh
$ git checkout fb-newbranch
$ git push --set-upstream origin fb-newbranch
$ git checkout develop
$ git reset --hard HEAD~1
```

Commande chaîné :
```sh
$ git <command> && git <commande> && ...
```

## Helpfull link
> https://git-scm.com/doc

> http://nvie.com/posts/a-successful-git-branching-model/

> http://learngitbranching.js.org/
