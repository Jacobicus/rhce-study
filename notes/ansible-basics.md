##Ansible

## Inventory
List of servers that Ansible manages and organizes into groups. The playbook that reads it knows where to run it from the inventory.

## Playbooks
These are executables that can tell one or multiple workstations at a time to run commands all at the same time. They run tasks in order and are written in YAML.

## Variables and group_vars
Variables get substituted into playbooks like package_name: httpd. Group_vars are files that store variables for a specific group of hosts so you do not hardcode values into playbooks.

## Handlers
Handlers trigger when a tasks makes a change. Example: If the config is changed, it restarts the service.

## Roles
Roles are a way to organize the playbook code into structured folders cleanly using tasks, handlers, templates, and defaults separated cleanly. It's about code organization and reusability and not about limiting which hosts are affected.

## Vault
THe vault is an encryption that stores a secret password that only be accessed by knowing a password. It is an AES256 encrypted file that stores sensitive data like passwords and API keys. It is encrypted at rest, and decrypted at runtime by Ansible when you provide the vault password. Secrets never sit in plaintext in code or Github.

