


Setup
=====


init
----


```
mkdir test.git
cd !#
git --bare init
```


clone
-----

* <http://stackoverflow.com/questions/791959/how-to-use-git-to-download-a-particular-tag>



* clone the repository ...
```
git clone https://github.com/FortAwesome/Font-Awesome.git
git clone https://github.com/rlong/emacs.d
```



tags
====


create
------

* create a tag:
```
git tag -a 0.3.2.1 -m 'iteration 3.2'
git tag -a 2015.8.24.2 -m '2015.8.24.2'
```

* push tags after they are committed:
```
git push --tags
```


list (read)
-----------

list the tags …
```
git tag -l
```

switching
---------

```
git checkout tags/0.3.2.1
git checkout tags/v3.0.2
```



Submodules
==========


```
git submodule add https://github.com/rlong/cocoa.lib.NodeTree
```
