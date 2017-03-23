# nycjv321's Development Environment a la carte

This repository contains playbooks automating various components of my development enviroment built on top of Fedora

## General Apps
* Atom
* Chrome
* htop
* vim
* wget

## Source Control
* Git
* GitKraken

## Languages
* Oracle JDK 1.8
* Ruby via RVM
* Golang (1.6.x)
* Node (v6.x)

## IDEs
* IntelliJ
* RubyMine 
* DataGrip
* WebStorm
* PyCharm
* CLion

## Usage

Configure your hosts in `/etc/ansible/hosts`. The playbooks are configured to run against localhost and "vms".
So something like:

	[vms]
        $host_ip ansible_user=$ansible_user

Run a playbook:

	ansible-playbook playbook.yml -k --extra-vars='ansible_become_pass=$ansible_user_pass'
