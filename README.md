# Ansible Role: sysstat

An Ansible role that deploys and configures [sysstat][01] on Linux boxes.

## 🚀 Motivation

From sysstat's [GitHub repository][01]:

*The sysstat package contains various utilities, common to many commercial Unixes, to monitor system performance and usage activity.*

This role deploys [systat][01] and configures it to automatically collect and historize performance and activity data.

## 📑 Role Variables

Check [here][02].

## 🧰 Dependencies

None.

## ⚡ Quick start

An example of how integrate this role to an Ansible playbook can be found here:

```yml
---
- name: Deploy sysstat
  hosts: all
  become: true
  gather_facts: true
  roles:
    - fernandobohrer.sysstat
```

## ⚙️ Compatibility

This role was tested on and is confirmed to work with the following Linux distributions:

- `Debian 12`
- `Ubuntu 22.04`
- `Ubuntu 24.04`

Details can be found in the [Molecule][03] scenarios available in the `molecule` folder.

## ⚠️ Warning

This Ansible role was tested on the above mentioned Linux distributions considering their default configuration. Your environment might have a different configuration or requirements which might conflict with the options that this role uses.

With the above in mind, it is **imperative** that you familiarize yourself with what this role does and test it on non-production machines **before** applying it to machines in a production environment.

## 📝 License

This project is licensed under the terms of the [MIT license][04].

[01]: https://github.com/sysstat/sysstat
[02]: defaults/main.yml
[03]: https://github.com/fernandobohrer/ansible-molecule-scenarios
[04]: /LICENSE
