# Qubes OS General

## Avoid Blue light

### Redshift

Install in dom0:
* `sudo qubes-dom0-update --enablerepo=qubes-dom0-current-testing redshift-gtk`

In anotherVM, download the config file:
* `wget https://raw.githubusercontent.com/csriq/qubes-os-usage/master/configs/redshift.conf`
* The file is the same as in http://jonls.dk/redshift/

In dom0, copy the config file from anotherVM to dom0:
* `qvm-run --pass-io anotherVM 'cat /path/to/redshift.conf' > ~/.config/redshift.conf`
