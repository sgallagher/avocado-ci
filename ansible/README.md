# Ansible Playbook For configuring Avocado
To use this playbook, create a file in the current directory called `hosts`
containing the following content:

```
hostname.fqdn ansible_ssh_user=root ansible_ssh_pass=<REDACTED>
```

You can specify any number of hosts that you want in this file. The password
may be skipped if SSH keys have been set up instead.

## Running the playbook
`ansible -i hosts demo-play.yml`

## Limitations
Currently, this playbook only works on Fedora 24 and Fedora 25.
