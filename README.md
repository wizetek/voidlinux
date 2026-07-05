# About

[Void Linux](https://voidlinux.org/) [XBPS](https://docs.voidlinux.org/xbps/) wrapper providing conventional syntax similar to Debian's `apt` and Fedora's `dnf`

# Syntax

`xbps <command> [arguments]`

Example:

`xbps install vim`

# Usage

```
xbps
      check                -Mun
      sync         (ref)
      update       (up)    -Su
      orphans
      clean
      status               -l
      list         (ls)
      available    (la)
      all          (ll)
      manual       (lm)    -m
      repos        (lr)    -L

      install      (in)
      reinstall    (re)
      remove       (rm)
      removeonly   (ro)
      configure    (cfg)
      hold
      unhold
      setauto
      setmanual
      search       (se)    -Rs
      searchlocal  (sl)    -s
      show         (info)  -RS
      showlocal            -S
      files                -Rf
      fileslocal           -f
      owns                 -o
      deps                 -x
      revdeps              -X

XBPS: 0.60.7 API: 20250629 GIT: UNSET
```

## Aliases

Whole words, partials words, shorthands, and `-` options can be used

```
check
sync | refresh | ref
update | upgrade | up
orphans | orphan | removeorphans
clean | cleancache | wipe
status
list | listinstalled | ls
available | listavailable | la
all | listall | ll
manual | listmanual | lm
repos | repo | listrepos | listrepo | repolist | lr
install | inst | in | add
reinstall | reinst | re
remove | rem | rm | uninstall | uninst | un | delete | del | erase
removeonly | ro
configure | conf | reconfigure | reconf | cfg
hold
unhold
setauto
setmanual
search | se
searchlocal
show | details | detail | info | inf
showlocal
files | file
fileslocal | filelocal
owns | own
deps | dep | depends
revdeps | revdep | revdepends | rdeps | rdep | rdepends
```

Example:

`xbps update` is the same as `xbps up` is the same as `xbps -Su`

`xbps refresh` is the same as `xbps ref` is the same as `xbps sync`

`xbps uninstall nano` is the same as `xbps remove nano` is the same as `xbps rm nano`

`xbps -s htop` is equivalent to `xbps searchlocal htop`
