


Setup
=====


init
----


```
mkdir test.git
cd !#
git --bare init
```





Branches
========



Tags
====


create
------

Create a tag:
```
git tag -a 0.3.2.1 -m 'iteration 3.2'
git tag -a 2015.8.24.2 -m '2015.8.24.2'
```

Push tags after they are committed:
```
git push --tags
```


list (read)
-----------

List the tags:
```
git tag -l
```


commands
========

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

`diff`
------


Changes associated with a commit
```
git diff dd71151623eb9c5edb1a89043acd608936596bbc^!
```


`submodule`
-----------


```
git submodule add https://github.com/rlong/cocoa.lib.NodeTree
```
