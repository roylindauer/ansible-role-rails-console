# Ansible Role - Rails Console

Based on a thing I did while working for Blackbird Logistics.

This ansible playbook creates rails console accounts that would allow users to ssh into an Ops VM
and connect directly to a ruby on rails console for a specific envirionment. 
Ops was a small VM behind a VPN for emergency interaction
with Rails. Access was based on which user group they belonged to, so if you were in `engineers` you had 
access to develop and staging, `production_engineers` you could connect to prod. `admin` had access to
all things.

The user could `ssh develop@ops` and get dropped into a rails console in the develop environment. 
