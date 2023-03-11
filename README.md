# Ansible Role: rpi_setup

An Ansible Role that configure [Raspberry Pi](https://www.raspberrypi.com) with [Raspberry Pi OS](https://www.raspberrypi.com/software/).

To install Raspberry Pi OS in the SD card the official tool [Raspberry Pi Imager](https://github.com/raspberrypi/rpi-imager) is available.

## Requirements

Requirements listed in `requirements.yml` file, installable via Ansible-Galaxy with the following command:

    ansible-galaxy install -r requirements.yml

## Role Variables

Available variables listed in `defaults/main.yml` file.

## Example Playbook

```yaml
- hosts: rpi
  gather_facts: false
  become: true
  vars_files:
    - rpi_configs.yml
  roles:
    - realgreendragon.rpi_setup
```

## License

GPLv3
