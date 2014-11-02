go-playbook
===========

Ansible playbook that installs golang from source for your plateform and set all path with bells and whistles


Prerequisites :
- pip. (optionnal)
- ansible. To install:   $ pip install ansible
- make tools + gcc or clang

To install on localhost, just run
```
$ sudo ansible-playbook site.yml
```

(as I write this file) The current go stable version is 1.3.3.

But, if you want use newer stable releases (in the future), open http://golang.org/dl/ check version number like x.y.z in go1.3.3.src.tar.gz for example and replace it at this file group_vars/all changing :
```
go_version: 1.3.3
```
to
```
go_version: x.y.z
```
