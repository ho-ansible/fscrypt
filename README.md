# Ansible role: fscrypt
File-based encryption on existing ext4 filesystem

## Requirements
Ext4 filesystem and recent kernel with `CONFIG_FS_ENCRYPTION`.
Only tested on Debian stable, for now.

## Role Variables
+ `fscrypt_dirs`: list of paths on which to enable encryption.
  Must be empty prior to encrypting.

## Playbooks
+ `main.yml`: apply role
+ `uninstall.yml`: remove. Run prior to removing host from inventory group.

## Dependencies
None.

## License
+ Ansible role licensed [MIT](LICENSE)

## Author Information
+ Ansible role by [Sean Ho](https://github.com/ho-ansible/)
