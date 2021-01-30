# Role Name

Install and maintain system-wide Fetchmail configuration.

## Requirements

None.

## Role Variables

Default variables are set in `defaults/main.yml`.

## Dependencies

No dependency on other Ansible Galaxy roles.

## Example Playbook

    - hosts: servers
      vars:
        fetchmail_config: |
          poll imap.gmail.com protocol IMAP
            user "example@gmail.com" is johndoe here
            password 'mysecretpassword'
            folder 'BUP'
            fetchlimit 1
            keep
            ssl
      roles:
        - hspaans.fetchamil

## License

MIT

## Author Information

This role was created in 2021 by [Hans Spaans](https://github.com/hspaans).
