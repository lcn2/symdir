# symdir

make a directory with links to files under a tree


# To install

```sh
sudo make install
```


# Example

```sh
$ mkdir /tmp/destdir
$ /usr/local/bin/symdir /usr/local/src/bin/symdir /tmp/destdir
$ ls -lRa /tmp/destdir
```


# To use

```
/usr/local/bin/symdir [-h] [-v lvl] [-V] [-n] [-a] [-g perl_exp] [-i] srcdir destdir

	-h	     print this help message
	-v lvl 	     verbose / debug level
	-V	     print version and exit

	-n	     do not anything, just print cmds (def: form symlinks)

	-a	     don't abort/exit after a fatal error (def: do)
	-g perl_exp  only form paths that match the Perl regexp (def: for all)
	-i	     ignore case when processing perl_exp (def: don't)

	srcdir	     source directory of file tree
	destdir	     destination directory where symlins are formed

    NOTE:
	exit 0	all is OK
	exit >1 some fatal error

symdir version: 1.2.1 2025-03-25
```


# Reporting Security Issues

To report a security issue, please visit "[Reporting Security Issues](https://github.com/lcn2/symdir/security/policy)".
