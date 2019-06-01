# Qubes OS General

## Avoid Blue light

### Redshift

Install in dom0:
* `sudo qubes-dom0-update --enablerepo=qubes-dom0-current-testing redshift-gtk`

In anotherVM, download the config file:
* `wget https://raw.githubusercontent.com/csriq/qubes-os-usage/master/configs/redshift.conf`
* The file is like in http://jonls.dk/redshift/ , but with changed screen=0,transition=0 and always the same night screen temperature 2800. You can chage those if you want to. Alternatively, search for other [redshift.conf files in GitHub](https://github.com/search?q=redshift.conf).

In dom0, copy the config file from anotherVM to dom0:
* `qvm-run --pass-io anotherVM 'cat /path/to/redshift.conf' > ~/.config/redshift.conf`

Test it and if desired make some changes to redshift.conf:
* `redshift`
