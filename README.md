# noobient.gitconfig

## Synopsys

This role lets you set Git config options.

## Parameters

| Name | Required | Example | Description |
|---|---|---|---|
| `name` | yes | `user.name` | Git config option name. |
| `value` | yes | `Stewie Griffin` | Git config option vale. |
| `scope` | no | `global` | Git config option scope. Possible values are `system` and `global`. Defaults to `system`. |
| `conflict` | no | `Eric Cartman` | Don't change the specified option, if its current value is this. |

## Examples

```yml
- include_role:
    name: noobient.gitconfig
  vars:
    name: 'user.name'
    value: 'Stewie Griffin'

- include_role:
    name: noobient.gitconfig
  vars:
    name: 'user.name'
    value: 'Eric Cartman'
    scope: 'global'
    conflict: 'Stewie Griffin'
```

## Return Values

N/A

## Support

| Platform | Support | Status |
|---|---|---|
| Linter | ✅ | [![Lint](https://github.com/noobient/ansible-galaxy-gitconfig/actions/workflows/lint.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-gitconfig/actions/workflows/lint.yml) |
| AlmaLinux 8 | ✅ | [![AlmaLinux 8](https://github.com/noobient/ansible-galaxy-gitconfig/actions/workflows/almalinux-8.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-gitconfig/actions/workflows/almalinux-8.yml) |
| AlmaLinux 9 | ✅ | [![AlmaLinux 9](https://github.com/noobient/ansible-galaxy-gitconfig/actions/workflows/almalinux-9.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-gitconfig/actions/workflows/almalinux-9.yml) |
| Fedora 40 | ✅ | [![Fedora 40](https://github.com/noobient/ansible-galaxy-gitconfig/actions/workflows/fedora-40.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-gitconfig/actions/workflows/fedora-40.yml) |
| Fedora 41 | ✅ | [![Fedora 41](https://github.com/noobient/ansible-galaxy-gitconfig/actions/workflows/fedora-41.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-gitconfig/actions/workflows/fedora-41.yml) |
| Ubuntu 20.04 | ✅ | [![Ubuntu 20.04](https://github.com/noobient/ansible-galaxy-gitconfig/actions/workflows/ubuntu-20.04.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-gitconfig/actions/workflows/ubuntu-20.04.yml) |
| Ubuntu 22.04 | ✅ | [![Ubuntu 22.04](https://github.com/noobient/ansible-galaxy-gitconfig/actions/workflows/ubuntu-22.04.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-gitconfig/actions/workflows/ubuntu-22.04.yml) |
| Ubuntu 24.04 | ✅ | [![Ubuntu 24.04](https://github.com/noobient/ansible-galaxy-gitconfig/actions/workflows/ubuntu-24.04.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-gitconfig/actions/workflows/ubuntu-24.04.yml) |
