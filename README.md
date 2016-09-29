# TACACS+ (Terminal Access Controller Access Control System plus)

C Daemon that authenticates requests via the Tacacs+ Protocol and logs accounting information.

This is a fork of Cisco + Shruberry's Tacacas+ daemons [tac_plus](http://www.shrubbery.net/tac_plus/).


## Requirements
- Linux (have not tested in other OSs)
- tcpwrappers(-devel)


## INSTALLING
```
cd tacacs+
./configure --enable-maxsess [--prefix=<basedir>]
#By default, All tac_plus crud will be installed under /usr/local.
#This can be overridden with the --prefix option.  E.g.:

 ./configure --prefix=/usr/pkg

#see ./configure --help for other configure options.

#you need ./configure with --enable-maxsess option, otherwise you may meet the following error:
	maxsessint.c: In function ¡®maxsess_check_count¡¯:
	maxsessint.c:60:51: error: ¡®S_maxsess¡¯ undeclared (first use in this function)
	   maxsess = cfg_get_intvalue(user, TAC_IS_USER, S_maxsess, TAC_PLUS_RECURSE);
	   	                                             ^
	maxsessint.c:60:51: note: each undeclared identifier is reported only once for each function it appears in

make install
```
more details see [INSTALL](./tacacs+/INSTALL)

Hope you will enjoy it ;)
