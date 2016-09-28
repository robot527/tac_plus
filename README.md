# TACACS+ (Terminal Access Controller Access Control System plus)

C Daemon that authenticates requests via the Tacacs+ Protocol and logs accounting information.

This is a fork of Cisco + Shruberry's Tacacas+ daemons [tac_plus](http://www.shrubbery.net/tac_plus/).


## Requirements
- Linux (have not tested in other OSs)
- tcpwrappers(-devel)


## INSTALLING
```
cd tacacs+
./configure [--prefix=<basedir>]
#By default, All tac_plus crud will be installed under /usr/local.
#This can be overridden with the --prefix option.  E.g.:

 ./configure --prefix=/usr/pkg

#see ./configure --help for other configure options.

make install
```
more details see [INSTALL](./tacacs+/INSTALL)

Hope you will enjoy it ;)
