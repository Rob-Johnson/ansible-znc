# ansible-znc

An ansible role used to run a ZNC docker container.

## Vars

Defaults are provided for all vars in `defaults/main.yml`

- `znc_user` Username for ZNC
- `znc_password` Password for ZNC
- `znc_docker_repo` Git repo from which your ZNC image can be built. Example (here)[https://github.com/shykes/docker-znc] and (here)[https://github.com/Rob-Johnson/docker-znc]
- `build_dir`: /tmp/docker-images/znc - The directory in which to build the image
- `image_tag`: znc - the tag with which to build the container
- `container_name`: znc - the name with which to run the container

### To Run

- Include the ansible role in your playbook.

```yaml

- hosts: all
  sudo: True
  roles:
    - znc
```
