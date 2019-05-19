# **Ansible-Jenkins**

Ansible-Jenkins is an Ansible role to install and configure Jenkins.

## **Requirements**

At the moment this role is being written for Debian based distributions e.g. Debian/Ubuntu. It will evolve to include other major distributions.

## **Role Variables**

## **Dependencies**

This role doesn't depends on any other role for execution.

## **Example Playbook**

Facts gathering must be enabled.

An example of running the role is as follows:
```yml
- hosts: servers
  gather_facts: True
  roles:
      - Ansible-Jenkins
```
## **License**

This role is licensed under MIT License (See the LICENSE file).

## **Author**

[Saad Ali](https://github.com/nixknight)
