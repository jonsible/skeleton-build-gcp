# {{ cookiecutter._organization }}.{{ cookiecutter.role_name }}

[![Build Status](https://travis-ci.com/{{ cookiecutter._organization }}/{{ cookiecutter.role_name }}.svg?branch=master)](https://travis-ci.com/{{ cookiecutter._organization }}/{{ cookiecutter.role_name }})
[![Galaxy](https://img.shields.io/badge/galaxy-{{ cookiecutter._organization }}.{{ cookiecutter.role_name }}-blue.svg)](https://galaxy.ansible.com/{{ cookiecutter._organization }}/{{ cookiecutter.role_name }}/)

{{ cookiecutter.description }}

## Requirements

None.

## Role Variables

### Default usage

As default {{ cookiecutter.role_name }} is installed and running.
If you want to adapt this to your needs look at the [Advanced usage](#advanced-usage) section.

### Advanced usage

For more advanced usage the following variables are available:
```yaml
{{ cookiecutter.role_name }}_source_path: "{{'{{'}} global_source_path | default('/opt') {{'}}'}}"
{{ cookiecutter.role_name }}_prefix: "{{'{{'}} global_prefix | default('/usr/local') {{'}}'}}"
{{ cookiecutter.role_name }}_user_install: "{{'{{'}} global_user_install | default(false) {{'}}'}}"
{{ cookiecutter.role_name }}_user_config: "{{'{{'}}_global_user_config | default(false) {{'}}'}}"
{{ cookiecutter.role_name }}_skel_config: "{{'{{'}} global_skel_config | default(false) {{'}}'}}"
{{ cookiecutter.role_name }}_install_from_source: "{{'{{'}} global_install_from_source | default(false) {{'}}'}}"
{{ cookiecutter.role_name }}_force_install: "{{'{{'}} global_force_install | default(false) {{'}}'}}"
{{ cookiecutter.role_name }}_user_strip: "{{'{{'}} global_user_strip | default([]) {{'}}'}}"
{{ cookiecutter.role_name }}_user_filter: "{{'{{'}} global_user_filter | default([]){{'}}'}}"
{{ cookiecutter.role_name }}_version: "2.9"
```

## Dependencies

None

## Example Playbook

Install {{ cookiecutter.role_name }} with the default settings
```yaml
- hosts: all
  roles:
     - role: {{ cookiecutter._organization }}.{{ cookiecutter.role_name }}
```

## License

GPL-3.0-or-later

## Author Information

This role was created in {{ cookiecutter._year }} by [{{ cookiecutter._author }}].
