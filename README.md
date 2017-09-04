# TestGithub

How to use git

### Branch
Créer une nouvelle branche :
> git checkout -b newBranch

Positionner le HEAD sur une branche :
> git checkout newBranch

### Commit
Ajouter les modification au commit :
> git add .

Créer un commit avec commentaire :
> git commit -m "Commit test"

### merge

Merge une branche sur la branche actuel avec ses historiques de commit :
> git merge  branchToMerge

Merge une branche sur la branche actuel sans ses historiques de commit :
> git merge --no-ff branchToMerge
