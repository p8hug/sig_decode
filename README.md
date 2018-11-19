# sig_decode
This repository contains some [sigrok](https://sigrok.org) decoders.

Sigrok comes with a command line interface called sigrok-cli and a viewer called pulseview. Both can be downloaded from the sigrok website.

# How to install decoders
Basically there are two options for installations:
1. Copy the required decoder into the installation directory of both sigrok-cli and pulseview.
1. Create for each decoder a link into your local copy of this repository.

## Create link on windows
The following steps are required:
1. Start command prompt as administrator
1. Create a directory junction

Examples:

Example for sigrok-cli:

> mklink /J "c:\Program Files (x86)\sigrok\sigrok-cli\share\libsigrokdecode\decoders\<decoder_xy>" "c:\<repository>\<decoder_xy>\"

Example for pulseview:

> mklink /J "c:\Program Files (x86)\sigrok\PulseView\share\libsigrokdecode\decoders\<decoder_xy>" "c:\<repository>\<decoder_xy>\"
