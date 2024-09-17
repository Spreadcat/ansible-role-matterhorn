# Role spreadcat.matterhorn

A simple Ansible role to setup matterhorn on the local machine and configure it.
It fetches the releases from the matterhorn GitHub page and installs it locally.

## Requirements

* `bunzip2`, `gunzip`, something like that can be used to unpack the release.

## Role Variables

For a list of role variables, defaults and how to use them check out the file `./defaults/main.yml`.

## Dependencies

* None

## Example Playbook

Including an example of how to use your role (for instance, with variables
passed in as parameters) is always nice for users too:

```yaml
- hosts: localhost
  gather_facts: false
  connection: local
  roles:
    - role: spreadcat.matterhorn
      matterhorn_mattermost_host: "www.example.com"
      matterhorn_mattermost_username: "jdoe"
      matterhorn_mattermost_password: "foobar"
```

## License

MIT

## Author Information

Written and maintained by [dbv](mailto:spreadcat.github@micronarrativ.org)
