# TestGithub

How to use git !

## Table des matières

[create an anchor](## Branch)
[create an anchor](## Commit)
[create an anchor](## Merge)
[create an anchor](## Helpfull link)


## Branch
Créer une nouvelle branche :
```sh
$ git checkout -b newBranch
```

Positionner le HEAD sur une branche :
```sh
$ git checkout newBranch
```

Mise à jour des branches depuis origine :
```sh
$ git fetch -all
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

## Helpfull link
> https://git-scm.com/doc

> http://nvie.com/posts/a-successful-git-branching-model/

> http://learngitbranching.js.org/
