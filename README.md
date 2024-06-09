# Usage

## Create files

```sh
$ cat <<EOF > /etc/ansible/hosts
[apt-hosts]
{HOSTNAME} ansible_user={USERNAME}

[yum-hosts]
{HOSTNAME} ansible_user={USERNAME}
EOF

$ cat <<EOF > /etc/ansible/ansible.cfg
[defaults]
log_path=/tmp/ansible.log
EOF
```

## Execute

```sh
# check syntax before execute
$ ansible-playbook *****.yml --syntax-check
# execute ansible playbook
$ ansible-playbook *****.yml
```
