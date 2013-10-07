##ansible-znc

Provision znc running in docker container

### Requirements
You need a group 'znc' in your $ANSIBLE_HOSTS, aswell as group|host variables docker_znc_repo, znc_user, znc_password

```bash
$ cat ansible_hosts
```
```yaml
[znc]
znc znc_user=foo znc_password=baz docker_znc_repo=https://github.com/Rob-Johnson/docker-znc.git
```

### To Run
```bash
$ ansible-playbook znc-playbook/site.yml
```




