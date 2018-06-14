# General

## merge-base
___

!!! note "merge-base finds the best common ancestor(s) between two commits."

	- useful for rebasing a stale branch onto master
    
### usage		

	X is a commit
	Y is the commit you want X to rebase onto

	git merge-base X Y
	546ae664634d9c44c
	git reset --soft 546ae664634d9c44c
	git commit -m "???"
	git rebase master

## commit --amend
___

!!! note "The --amend option is a convenient way to modify the most recent commit"

	- useful for changing the commit message of the previous commit without resetting
	- useful for squashing changes into the previous commit without resetting

### usage

	git commit --amend

!!! warning "will prompt you to open an editor"

To amend the previous commit with a new commit message without opening an editor use:
		
	git commit --amend -m "an updated commit message"

To simply squash staged changes into the previous commit without changing the commit message, use:

	git commit --amend --no-edit 