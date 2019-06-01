# Qubes OS Security

## Between Qubes

### Deny pasting into your vault.

In dom0:
* `sudo nano /etc/qubes-rpc/policy/qubes.ClipboardPaste`
* add the line: `$anyvm vault deny` above the line `$anyvm $anyvm ask`
