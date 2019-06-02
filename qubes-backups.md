# Qubes OS Backups

## Qubes Backup, Restoration, and Migration

Please look at the [official documentation](https://www.qubes-os.org/doc/backup-restore/).

Advantages:
* back up and restore your whole system
* migrate between two physical machines
* restore in any GNU/Linux system

Disadvantages:
* no incremental backups
* cannot backup only specific folders/files in the vm

## Incremental Backups
* [Sparsebak](https://github.com/tasket/sparsebak) - incremental backup management for logical volumes. In alpha/testing stage.
* [POC](https://github.com/v6ak/qubes-incremental-backup-poc) - Incremental Backup Proof of Concept for v3 (not v4)
