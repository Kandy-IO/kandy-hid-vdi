# @kandy-io/kandy-hid-vdi

The Kandy HID Toolkit is an optional library that abstracts HID device functions to the application developer in standard desktop and VDI environments. It is currently supported for Electron based WebRTC applications running on Windows and Mac desktops and on Citrix VDI with eLux thin clients.<br>

The Kandy HID Toolkit enables application developers to handle HID device call operations.<br>

The Kandy HID Toolkit is currently supported with several Jabra headsets, with support for HID devices from other vendors possible.

This repository contains the Citrix Plugin for the Kandy HID Toolkit.

In order to use this software the [corresponding Javascript SDK](https://github.com/Kandy-IO/kandy-hid-sdk) is also required.

## Installation

This software is delivered in the form of eLux distribution packages. See documentation for your version of Citrix Workspace.

## Logging

Once installed, logs generated from by the DLL are written to syslog and so can be observed in /var/log/messages. They have a prefix of `VDIHID:`

## Disabling the DLL

In a Citrix VDI configuration, the DLL can be disabled (prevented from loading) by modifying /setup/kandy.ini on the eLux Thin Client and setting RTC_HID to Off:

```
[Modules]
RTC_HID=Off
```
Note that this will prevent the kandy-hid-sdk running in the container/web app from communicating with HID devices.

## Known Issues / Limitations
- the Jabra Speak 710 is known to conflict with either the mouse or keyboard when offhook. A support ticket (299) has been created with the device vendor

## CHANGELOG
See [CHANGELOG](./CHANGELOG.md).
