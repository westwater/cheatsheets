# General

## Difficulities rebasing
___

In a situation when you are working on a branch that has been off master for a while and haven't been rebasing, instead of using 

	git rebase master

use

	git merge-base X Y
	546ae664634d9c44c
	git reset --soft 546ae664634d9c44c
	git commit -m "???"
	git rebase master

!!! note
    merge-base finds the best common ancestor(s) between two commits.
