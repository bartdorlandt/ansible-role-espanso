# espanso
This role will install espanso using homebrew under MacOSX.

It will link the configuration directories to a folder in your iCloud folder. 

* If they folder doesn't exist they will be created and filled with the default content, if existed.
* If they do exist, the default espanso configuration will be moved and a symlink created.
* 


## Requirements
- Homebrew installed
- No sudo password required

## Role Variables
Available variables are listed below, along with default values (see defaults/main.yml):

    dictionary:
      key1: "value1"
      key2: true

## Dependencies

* homebrew

## Example Playbook

    - hosts: localhost
      tasks:
        - name: espanso
          ansible.builtin.include_role:
            name: bartdorlandt.espanso

or:

    - hosts: localhost
      roles:
        - role: bartdorlandt.espanso
          vars:
            key1: false
            key2: "very special string"

## License

MIT/BSD

## Author Information

This role was created in 2024 by Bart Dorlandt.
