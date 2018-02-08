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
$ git branch <branche_name>
```

Positionner le HEAD sur une branche :
```sh
$ git checkout <branche_name>
```

Créer une nouvelle branche et positionner le HEAD sur cette branche
```sh
$ git checkout -b <branche_name>
```

Lister toute les branche remote + local
```sh
$ git branch -a
```

Suppression d'une branche et push vers origin:
```sh
$ git branch -d fb-branch
$ git push origin :fb-branch
```

## Commit
Ajouter les modifications dans le staging area
```sh
$ git add .
```

Commit la staging area avec un commentaire
```sh
$ git commit -m "Commit test"
```

## Merge

Déplace le HEAD sur une suite de commit d'une branche source en partant de la branche actuel
```sh
$ git merge [--ff] <branche_source>
```

Effectue un commit de fusion entre deux branche
```sh
$ git merge --no-ff branchToMerge
```

Mise à jours de la branche actuel par rapport à une autres :
```sh
$ git rebase origin/branchSource
```

## Other

Rajouter un remote et push une branch :
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

> https://www.miximum.fr/blog/enfin-comprendre-git/
