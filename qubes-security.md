# Qubes OS Security

## In single Qube

* [Qubes-VM-hardening](https://github.com/tasket/Qubes-VM-hardening)

## Between Qubes

### Deny pasting into your vault.

In dom0:
* `sudo nano /etc/qubes-rpc/policy/qubes.ClipboardPaste`
* add the line: `$anyvm vault deny` above the line `$anyvm $anyvm ask`
