# postfix [![Ansible Role](https://img.shields.io/ansible/role/d/cornfeedhobo/postfix)](https://galaxy.ansible.com/cornfeedhobo/postfix)

Install and configure postfix mail transfer agent

## Table of content

- [Requirements](#requirements)
- [Default Variables](#default-variables)
  - [postfix_aliases](#postfix_aliases)
  - [postfix_bin_path](#postfix_bin_path)
  - [postfix_config_dir](#postfix_config_dir)
  - [postfix_config_main](#postfix_config_main)
  - [postfix_config_master](#postfix_config_master)
  - [postfix_configure](#postfix_configure)
  - [postfix_group](#postfix_group)
  - [postfix_install](#postfix_install)
  - [postfix_owner](#postfix_owner)
  - [postfix_package_state](#postfix_package_state)
  - [postfix_packages](#postfix_packages)
  - [postfix_service](#postfix_service)
  - [postfix_service_enabled](#postfix_service_enabled)
  - [postfix_service_name](#postfix_service_name)
  - [postfix_service_state](#postfix_service_state)
  - [postfix_ssl](#postfix_ssl)
  - [postfix_ssl_dir](#postfix_ssl_dir)
  - [postfix_ssl_pair](#postfix_ssl_pair)
- [Discovered Tags](#discovered-tags)
- [Dependencies](#dependencies)
- [License](#license)
- [Author](#author)

---

## Requirements

- Minimum Ansible version: `2.9`

## Default Variables

### postfix_aliases

See man page for more https://man7.org/linux/man-pages/man5/aliases.5.html

#### Default value

```YAML
postfix_aliases: {}
```

#### Example usage

```YAML
postfix_aliases:
  root: "adminuser, /etc/motd"
```

### postfix_bin_path

#### Default value

```YAML
postfix_bin_path: '{{ __postfix_bin_path }}'
```

### postfix_config_dir

#### Default value

```YAML
postfix_config_dir: '{{ __postfix_config_dir }}'
```

### postfix_config_main

#### Default value

```YAML
postfix_config_main: ''
```

### postfix_config_master

#### Default value

```YAML
postfix_config_master: ''
```

### postfix_configure

#### Default value

```YAML
postfix_configure: false
```

### postfix_group

#### Default value

```YAML
postfix_group: '{{ __postfix_group }}'
```

### postfix_install

#### Default value

```YAML
postfix_install: false
```

### postfix_owner

#### Default value

```YAML
postfix_owner: '{{ __postfix_owner }}'
```

### postfix_package_state

#### Default value

```YAML
postfix_package_state: present
```

### postfix_packages

#### Default value

```YAML
postfix_packages: '{{ __postfix_packages }}'
```

### postfix_service

#### Default value

```YAML
postfix_service: false
```

### postfix_service_enabled

#### Default value

```YAML
postfix_service_enabled: true
```

### postfix_service_name

#### Default value

```YAML
postfix_service_name: '{{ __postfix_service_name }}'
```

### postfix_service_state

#### Default value

```YAML
postfix_service_state: started
```

### postfix_ssl

#### Default value

```YAML
postfix_ssl: false
```

### postfix_ssl_dir

#### Default value

```YAML
postfix_ssl_dir: '{{ __postfix_ssl_dir }}'
```

### postfix_ssl_pair

#### Default value

```YAML
postfix_ssl_pair:
  name: ''
  key: ''
  crt: ''
```

## Discovered Tags

**_postfix_**

**_postfix-configure_**

**_postfix-install_**

**_postfix-service_**

**_postfix-ssl_**


## Dependencies

None.

## License

MIT

## Author

cornfeedhobo
