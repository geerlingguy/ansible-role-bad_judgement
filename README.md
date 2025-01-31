# Bad Judgement

[![CI](https://github.com/geerlingguy/ansible-role-bad_judgement/actions/workflows/ci.yml/badge.svg)](https://github.com/geerlingguy/ansible-role-bad_judgement/actions/workflows/ci.yml)

**DO NOT USE THIS ROLE**. At least not in production. Or on any type of server you care about. Bad things will happen.

<img src="https://raw.githubusercontent.com/geerlingguy/ansible-role-bad_judgement/master/files/bad-judgement-pirates-of-the-caribbean.jpg" alt="A brilliant example of bad judgement; never trust a pirate." />

This role traces its lineage back to the [Bad Judgement](https://www.drupal.org/project/bad_judgement) module for Drupal. The basic premise is any other role which is never meant to run in production should require this role as a dependency. And then both roles should warn the user to never run them in production.

But why would someone ever publish a role on Ansible Galaxy if it's not meant to be used?

Well, there are two potential reasons:

  - As a joke (e.g. Drupal's [khaaaaaaan](https://www.drupal.org/project/khaaaaaaan) module)
  - For the purpose of demonstration by negative example (e.g. this role)

This role was originally created by [Jeff Geerling](https://www.jeffgeerling.com) for his AnsibleFest Austin 2019 presentation _There's a role for that! How to evaluate community roles for your playbooks_.

## Judgement vs Judgment

Did you know both spellings are considered correct? This project chose the 'older' spelling over the more common one we use in US English today.

But if you're going to argue more about this project's naming than the fact that you shouldn't be using this project in the first place, _you probably have bad judgement_ ;-)

## Requirements

  - Really bad judgement.

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

    preserve_files: true

Set this to `false` if you don't want to preserve files.

    preserve_files_dir: /tmp

Set this to the directory which stores temporary files you would like to preserve (or not) depending on the `preserve_files` setting.

Dependencies
------------

N/A

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: all
      roles:
         - role: geerlingguy.bad_judgement

License
-------

MIT / BSD

Author Information
------------------

This role was created in 2019 by [Jeff Geerling](https://www.jeffgeerling.com/), author of [Ansible for DevOps](https://www.ansiblefordevops.com/).

_Image from [Digital Domain - Pirates of the Caribbean: At World's End](https://www.digitaldomain.com/work/pirates-of-the-caribbean-at-worlds-end/)._
