# ansible-role-sizeup

[![Build Status](https://travis-ci.org/tkimball83/ansible-role-sizeup.svg?branch=master)](https://travis-ci.org/tkimball83/ansible-role-sizeup)

macOS - The Missing Window Manager

## Requirements

This role requires homebrew and homebrew cask to be installed

## Role Variables

Available variables are listed below, along with default values:

    sizeup_pkg: SizeUp
    sizeup_domain: "com.irradiatedsoftware.{{ sizeup_pkg }}"
    sizeup_defaults: {}

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

GPLv3

## Author Information

This role was created by [Taylor Kimball](http://www.linuxhq.org).
