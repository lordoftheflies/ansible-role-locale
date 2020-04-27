---
title: 'Role for locale'
description: 'Ansible Role for setup locales.'
---

# Ansible Role: Locale

Ansible Role for setup locales.

## Status

[![Build Status](https://travis-ci.org/lordoftheflies/ansible-role-locale.svg?branch=master)](https://travis-ci.org/lordoftheflies/ansible-role-locale)

[![Version](https://img.shields.io/github/v/tag/lordoftheflies/ansible-role-locale?sort=semver)](https://github.com/lordoftheflies/ansible-role-locale/releases)

![GitHub Release Date](https://img.shields.io/github/release-date/lordoftheflies/ansible-role-locale)

## Description

Locale is an Ansible Role used to setup and maintain production grade services.

## Roadmap

* [ROADMAP.md](ROADMAP.md)

## References

* [docs.ansible.com](https://docs.ansible.com/)
* [On Ansible Galaxy](https://galaxy.ansible.com/lordoftheflies/ansible_role_locale)

## Requirements

### Production

* Ansible

## Variables

<p>
<details>
<summary>ansible_role_locale_locales</summary>

List of presented locales, generate if needed.

Default: []

</details>
</p>

<p>
<details>
<summary>ansible_role_locale_default_language</summary>

Default locale language.

Default value: `en`

</details>
</p>

<p>
<details>
<summary>ansible_role_locale_default_variant</summary>

Default locale variant.

Default value: `US`

</details>
</p>

<p>
<details>
<summary>ansible_role_locale_default_encoding</summary>

Default locale encoding.

Default value: `UTF-8`

</details>
</p>


* [defaults/main.yml](defaults/main.yml) contains all of the required variables.

## Testing

### For Local Testing

* [Vagrant](https://www.vagrantup.com/) - (Tested using version 2.1.1)
* Vagrant plugins:
  * [vagrant-disksize (0.1.2)](https://github.com/<class 'jinja2.utils.Namespace'>/vagrant-disksize)
  * [vagrant-libvirt](https://github.com/<class 'jinja2.utils.Namespace'>/vagrant-libvirt)
  * vai (0.9.3) - For testing with multiple vms [vagrant-plugin-vai](https://github.com/<class 'jinja2.utils.Namespace'>/vagrant-plugin-vai)
  * [vagrant-vbguest (0.15.2) - Recommended vagrant-vbguest](https://github.com/<class 'jinja2.utils.Namespace'>/vagrant-vbguest)
* [Virtual Box](https://www.virtualbox.org/)
  * Tested using Version 5.2.14 r123301 (Qt5.6.1)

### Testing with Molecule

```shell
molecule test
```

### Testing with Vagrant

To test with all VM's defined in Vagrantfile run the following:

```shell
cd roles/locale
vagrant up
```

To run on a specific VM's
```shell
vagrant up xenial
```

## Authors

* This role was created in 2014 by [Jeff Geerling](https://www.jeffgeerling.com/), author of [Ansible for DevOps](https://www.ansiblefordevops.com/).
* Role upgraded in 2019 by [László Hegedűs](mailto:laszlo.hegedus@cherubits.hu), founder of [Cherubits LLC](https://portal.cherubits.hu)

## License

[Apache 2.0](https://tldrlegal.com/license/apache-license-2.0-(apache-2.0))

**NOTE**: Role generated using [ansible-role-skeleton](https://github.com/lordoftheflies/ansible-role-skeleton)
