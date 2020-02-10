---
x-masysma-name: internet-enable-disable
section: 32
title: Internet enable/disable
author: ["Linux-Fan, Ma_Sys.ma (Ma_Sys.ma@web.de)"]
keywords: ["internet", "ufw", "gufw", "firewall", "enable", "disable"]
date: 2019/12/21 01:00:53
lang: en-US
x-masysma-repository: https://www.github.com/m7a/lp-internet-enable-disable
x-masysma-website: https://masysma.lima-city.de/32/internet-enable-disable.xhtml
x-masysma-owned: 1
x-masysma-copyright: |
  Copyright (c) 2019 Ma_Sys.ma.
  For further info send an e-mail to Ma_Sys.ma@web.de.
---
Description
===========

Scripts to enable/disable internet access (outgoing access) by using the UFW
firewall. Provides an example sudo configuration which allows user `linux-fan`
to execute the scripts without passwords, giving the ability to temporarily
enable/disable internet access to the user. It is thus clear that this package
is intended only for _client-side usage_. `.desktop`-files are prvoided to
facilitate adding the scrips as buttons in desktop environments.

Files
=====

`55-masysma-internet-enable-disable`
:   Sudo-configuration which allows user `linux-fan` to
    run scripts `internet_enable` and `internet_disable` without password.
`internet_enable`
:   Run `/usr/sbin/ufw default allow outgoing`
`internet_disable`
:   Run `/usr/sbin/ufw default reject outgoing`
`internet_enable.desktop`
:   Shortcut for `sudo internet_enable`
`internet_disable.desktop`
:   Shortcut for `sudo internet_disable`
