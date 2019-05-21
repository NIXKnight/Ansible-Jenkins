# **Ansible-Jenkins**

Ansible-Jenkins is an Ansible role to install and configure Jenkins.

## **Requirements**

At the moment this role is being written for Debian based distributions e.g. Debian/Ubuntu. It will evolve to include other major distributions.

## **Role Variables**

`JENKINS_PREREQUISITE_PACKAGES` is used to defined requirements for installing a Jenkins server.

`JENKINS_REPO` defined Jenkins apt repository.

Using `JENKINS_OPEN_FILES`, you can modify the default ope files value in `/etc/default/jenkins`.

`JENKINS_HOST_IP` by, by default, set to the default IP address of the server.

`JENKINS_PORT` can be used to modify port.

`JENKINS_URL` is the URL of Jenkins which is made up of `JENKINS_HOST_IP` and `JENKINS_PORT`.

`JENKINS_JAVA_ARGS` defines `JAVA_ARGS` variable in `/etc/default/jenkins`.

`JENKINS_ARGS` defines `JENKINS_ARGS` variable in `/etc/default/jenkins`.

`JENKINS_USERS` defines users with administrative access to Jenkins.

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
