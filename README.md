aosp-ethernet
=============

This repository is a collection of patches to Google's AOSP tree
that provide Ethernet support to Android.

The original support is based on the zork from Android-x86 project
(see ethernet.diff.tar.gz from http://www.android-x86.org/download page).

The goal of the patchset is to provide a complete Ethernet support to
AOSP, from low-level layers to applicative framework.
The patchset is hardware independant and only requires the Linux kernel
Ethernet driver to be available.

The work has been made publicly available by Alcatel-Lucent and is
courtesy of Fabien Brisset and Benjamin Zores.

The patchset provides the following features:
- Ethernet low-level layer support in AOSP's framework.
- Settings app modification to allow DHCP/Static configuration by user.
- Ethernet IP/MAC addresses display in Settings app.
- StatusBar modification to add Ethernet connectivity status.
- DNS support.
- HTTP proxy support.
- NTP support.
- Seamless Ethernet connectivity support for all apps, shortcuting WiFi.

Relevant implementation details have been presented in November 2012
at Embedded Linux Conference Europe, Barcelona.

See http://www.slideshare.net/gxben/elce-2012-dive-into-android-networking-adding-ethernet-connectivity
for additional details and specific information.

This patchset has been developed against Ice Cream Sandwich 4.0.4_r2.1 branch.
It has been fully validated, though its implementation is not neat.
The patchset sources are available in the ics/ directory.

Long term goal is to provide a "Google-compliant" implementation instead
of an evil hack and push that upstream for complete integration.

Long-term implementation is available (still as a draft so far)
for JellyBean 4.2_r1 branch within the jb/ directory.

Feel free to send remarks and suggestions to:
- Fabien Brisset <fbrisset@gmail.com>
- Benjamin Zores <benjamin.zores@gmail.com>

Happy Hacking !

