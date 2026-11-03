NOTE: this is a Work In Progress as of 20261101.

# What is freebsd/bugzilla-exp?

freebsd/bugzilla-exp is a set of changes and extensions for Bugzilla being used
by the FreeBSD project. Those usually map a Bugzilla source package layout
in a 1:1 fashion.

# How do I use it?

freebsd/bugzilla will refer to a certain bugzilla package from the FreeBSD
ports, in this case, the latest development one (devel/bugzilla521).

Thus, if you install devel/bugzilla521, you can simply copy
linimon/freebsd-bugzilla-exp over ${PREFIX}/www/bugzilla to have a Bugzilla implementation
that resembles what the FreeBSD project uses at
https://bugstest2.freebsd.org/bugzilla.

In short:

* cd /usr/ports/devel/bugzilla521 && make install clean
* Download the latest development linimon/freebsd-bugzilla-exp bits from linimon/freebsd-bugzilla/tree/freebsd-bugzilla-exp
* tar -C /usr/local/www/bugzilla --strip-components=1 -xjvf (filename).tar.gz
* cd /usr/local/www/bugzilla && checksetup.pl
