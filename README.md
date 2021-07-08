---
- hosts: all
  tasks:
   - name: Install Maven using Ansible
become: yes
apt:
name: "{{ packages }}"
state: present
vars:
packages:
- maven
