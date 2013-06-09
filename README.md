hypercube
=========

Hypercube was the original tracker software developed by anakata (Gottfrid Svartholm) for [The Pirate Bay](http://thepiratebay.sx/).
Until today there was no trace of the project on Github. Problem solved !

Have fun.

***

Original README file :

```no-highlight
<beak> hypercube är ungefär som rap på skånska
<beak> coolt men lite skumt
```

How to compile (no autoconf, sorry...):
 - Edit asio/asio.h and select what async I/O interface you wanna use.
 - Edit Makefile.
   - If you are on Linux, USE_LINUX_SENDFILE should be defined.
   - If you are on Linux, using epoll (kernel >=2.6), and have a libc which
     doesn't support them (warnings about 'epoll_* is not implemented and
     will always fail' on linking), uncomment the AKEPOLL* lines.
 - Maybe put that final touch to config.h.
   It ships with DEBUG enabled. You probably want to disable this.

Now make :-).
The rest of the configuration is in your CFG_FILE (hypercube.cfg by
default).

 - anakata@anakata.hack.se || anakata@g-con.org
