# ansible-role-sizeup

[![Build Status](https://travis-ci.org/tkimball83/ansible-role-sizeup.svg?branch=master)](https://travis-ci.org/tkimball83/ansible-role-sizeup)
[![Ansible Galaxy](https://img.shields.io/badge/ansible--galaxy-sizeup-blue.svg?style=flat)](https://galaxy.ansible.com/tkimball83/sizeup)
[![License](https://img.shields.io/badge/license-GPLv3-brightgreen.svg?style=flat)](COPYING)

macOS - The Missing Window Manager

## Requirements

This role requires homebrew and homebrew cask to be installed

## Role Variables

Available variables are listed below, along with default values:

    sizeup_defaults: {}
    sizeup_domain: "com.irradiatedsoftware.{{ sizeup_package }}"
    sizeup_package: SizeUp

## Dependencies

None

## Example Playbook

    - hosts: localhost
      connection: local
      roles:
        - role: tkimball83.sizeup
          sizeup_defaults:
            CenterNonResizableWindows:
              type: bool
              value: true
            KeepWindowsInBounds:
              type: bool
              value: true
            MenuEnabled:
              type: bool
              value: true
            MultiMonitorResizeWindowProportionally:
              type: bool
              value: true
            SUEnableAutomaticChecks:
              type: bool
              value: true
            ShortcutsDisabled:
              type: bool
              value: false
            ShowOverlay:
              type: bool
              value: true
            ShowPrefsOnLaunch:
              type: bool
              value: false
            ShowPrefsOnNextStart:
              type: bool
              value: false
            ShowTooltips:
              type: bool
              value: false
            TakeDrawersIntoAccount:
              type: bool
              value: true
            suppressMenuBarDisabledPopup:
              type: bool
              value: true

## License

Copyright (C) 2018 Taylor Kimball <tkimball@linuxhq.org>

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program. If not, see <http://www.gnu.org/licenses/>.
