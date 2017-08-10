


Setup
=====








commands
========


`branch`
--------

* create a branch:
```
git branch testing
```

* create a branch from a specific commit:
```
git branch testing e2cbd43c4d352d6955fd214f20c48cad5f6b6b97
```

* delete a branch:
```
git branch -D xcode-7
```

* switch to a branch:
```
git checkout testing
# might need to do a reset ... http://stackoverflow.com/questions/3885850/git-not-removing-files-when-switching-branch
git reset --hard
git clean -f -d
```


`checkout`
----------

Revert a change:
```
git checkout -- client/css/base.css
```


Switching based on tags:
```
git checkout tags/0.3.2.1
git checkout tags/v3.0.2
```

`clone`
-------

* <http://stackoverflow.com/questions/791959/how-to-use-git-to-download-a-particular-tag>


* clone the repository ...
```
git clone https://github.com/FortAwesome/Font-Awesome.git
git clone https://github.com/rlong/emacs.d
```


`config`
--------


cache config for 24 hours (https://help.github.com/articles/caching-your-github-password-in-git/)

```
git config --global credential.helper cache
git config --global credential.helper 'cache --timeout=86400'
```

`clone`
=======

* clone over ssh (http://stackoverflow.com/questions/14348874/git-repository-url-ssh-syntax-without-absolute-path) ...
```
git clone ssh://login@server.com:12345/~/repository.git
```

`diff`
------


Changes associated with a commit
```
git diff dd71151623eb9c5edb1a89043acd608936596bbc^!
```

`log`
-----

* last commit on current branch
```
git log -n 1
```

* pictoral representation of git branches
```
git log --graph --oneline --all
```

`merge`
-------

* merging ...
```
git merge testing
```

`remote`
--------

add:
```
git remote add github https://github.com/johnezang/JSONKit.git
```

list:
```
git remote -v
```

rename:
```
git remote rename origin github
```


`submodule`
-----------

add:
```
git submodule add https://github.com/rlong/cocoa.lib.NodeTree
```

`tag`
-----


create:
```
git tag -a 0.3.2.1 -m 'iteration 3.2'
git tag -a 2015.8.24.2 -m '2015.8.24.2'
```

Push tags after they are committed:
```
git push --tags
```

list:
```
git tag -l
```


Cook Book
=========

initialise a bare repository
----------------------------

```
mkdir test.git
cd !$
git --bare init
```

rename a remote branch
----------------------

* [branch - git: renaming branches remotely? - Stack Overflow](https://stackoverflow.com/questions/4753888/git-renaming-branches-remotely)

```
git branch new-branch-name origin/old-branch-name
git push origin --set-upstream new-branch-name
git push origin :old-branch-name
```

clean up
```
git checkout new-branch-name
git fetch origin
git remote prune origin
```
