# Ansible Role: Plex

A role that installs [Plex Media Server](https://www.plex.tv)

## Requirements

None.

## Role Variables

```
# The Plex app support dir. This is where Plex stores thumbnails, poster art, etc.
# You might want to change this when running on (for example) a raspberry pi.
# Their SD cards are often to small, this directory can grow to some GB of data.
plex_app_support_dir: "/var/lib/plexmediaserver/Library/Application Support"

# The Linux user to run the plexmediaserver service as.
plex_service_user: "plex"

# The Linux user group to run the plexmediaserver service as.
plex_service_group: "plex"
```

## Dependencies

None.

## Example Playbook

```
- hosts: servers
  roles:
     - jelle_s.plex
```

## License

[MIT](https://raw.githubusercontent.com/Jelle-S/ansible_role_plex/master/LICENSE)

