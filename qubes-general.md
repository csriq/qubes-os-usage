# Qubes OS General

## VPN
* [How To make a VPN Gateway in Qubes](https://www.qubes-os.org/doc/vpn/) (official docs)
* [Qubes-vpn-support](https://github.com/tasket/Qubes-vpn-support)

## Avoid Blue Light

### Redshift

Install in dom0:
* `sudo qubes-dom0-update --enablerepo=qubes-dom0-current-testing redshift-gtk`

In anotherVM, download the config file:
* `wget https://raw.githubusercontent.com/csriq/qubes-os-usage/master/configs/redshift.conf`
* The file is like in http://jonls.dk/redshift/ , but with changed screen=0,transition=0,brightness=0.75 and always the same night screen temperature 2800. You can chage those if you want to. Alternatively, search for other [redshift.conf files in GitHub](https://github.com/search?q=redshift.conf).

In dom0, copy the config file from anotherVM to dom0:
* `qvm-run --pass-io anotherVM 'cat /path/to/redshift.conf' > ~/.config/redshift.conf`

Test it and if desired make some changes to redshift.conf:
* `redshift`

Add it as a startup application:
* `Menu -> System Tools -> Session and Startup -> Application Autostart` or `Alt+F3+startup+2xEnter -> Application Autostart`
* Click Add, enter 3x `redshift` and press OK

## Screen Sharing

Currently [possible](https://www.mail-archive.com/qubes-users@googlegroups.com/msg18236.html), but not without sacrificing security. Read the latest ideas [the mailinglist](https://www.mail-archive.com/qubes-users@googlegroups.com/msg18929.html).
