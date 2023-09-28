# Dev Laptop Setup

## Clone the git repository

```sh
xcode-select --install 2>/dev/null
cd ~
git clone https://github.com/DownRangeDevOps/laptop.git
```

## Adjust the Ansible playbook configuration

1. Copy `laptop/ansible/group_vars/defaults.yml` to `laptop/ansible/config.yml`
2. Edit `config.yml` to your liking

## Run the setup routine

```sh
cd laptop
./setup
```

## Optional post-setup tasks

* Generate an SSH key and add it to `ssh-agent` and your GitHub account
* Update the setup repository to use SSH:

```sh
git remote set-url origin git@github.com:DownRangeDevOps/laptop.git
```
