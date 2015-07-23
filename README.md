# Ansible Role: modman

An Ansible Role that installs `modman` - the Magento module     

## Role Variables

```
bennoislost_modman_download_url: "https://raw.githubusercontent.com/colinmollenhour/modman/master/modman"
```

URL to download `modman`. With this variable you can change the version number to use.

```
bennoislost_modman_bin_path: "/usr/bin/modman"
```
Path to executable - can be changed to a different location in your `$PATH`

## Example Playbook

```
- hosts: webservers
  vars_files:
    - vars/main.yml
  roles:
    - { role: bennoislost.modman }
```

## Roadmap

* Add `init`
* Add handers for `deploy-all, clean`
* Add hash to install from vcs

## License

MIT

## Thanks To

* Colin Mollenhour [link](https://github.com/colinmollenhour) & all contributors to the Project!
