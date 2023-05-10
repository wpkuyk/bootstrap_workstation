# bootstrap_workstation

Ansible playbook to bootstrap Linux workstation

---

## Initial Setup

Installing the latest Ansible is required before we can pull and run the play.

We need to install `git` before we can run `ansible-pull`.

``` bash
sudo apt install git
```

On Ubuntu, ensure the `python3-pip` module is installed.

``` bash
python3 -m pip -V
```

If the message is `No module named pip`, install with

``` bash
sudo apt install python3-pip
```

Then, install ansible for the current user

``` bash
python3 -m pip install --user ansible
```

This adds the ansible commands to /home/\<user\>/.local/bin, which needs to be added to $PATH.

``` bash
source ~/.profile
```

## Ansible-pull

``` bash
ansible-pull https://github.com/wpkuyk/bootstrap_workstation.git
```
