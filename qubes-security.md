# Qubes OS Security

## Between Qubes

Deny pasting into your vault:
* [@dom0 ~] `sudo nano /etc/qubes-rpc/policy/qubes.ClipboardPaste`
* [@dom0 ~] add the line: `$anyvm vault deny`
