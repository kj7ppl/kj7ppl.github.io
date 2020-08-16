---
layout: post
title:  "Secure Voice Using AFSK Modulation"
date:   2020-08-15 21:58:00 -0700
categories: crypto experiment
permalink: /secure-voice/
---
One of the things that finally prompted me to get an amateur radio license was
some experiments I was doing with secure voice. There are many commercial
systems that exist that require one replace their existing analog radio
infrastructure, such as P25 or DMR. This can be expensive, prohibitively so for
smaller organizations. And of course these systems would be useless over
non-radio voice mediums such as analog telephones.

I found an [open source voice codec](https://github.com/drowe67/codec2) that
used a low-bitrate AFSK scheme that was designed to function using narrow-band
voice FM, [modified it](https://github.com/aarmono/codec2) to encrypt the voice
packets, and [packaged it](https://github.com/aarmono/crypto_transceiver_instructions)
to run on a raspberry pi and some commodity USB audio devices so anyone could
use the system with minimal cost and no change to their existing radio
infrastructure.

Obscured communications are illegal on amateur bands, so this page serves as
documentation of how the communications are encoded and modulated so that
anyone may decode and understand the transmissions. The [key](/files/secure_voice_key)
I use for the transmissions is also provided here. If you follow the instructions
to format an SD card with the raspberry pi image, create a directory named
"config" on the SD card, and copy the key file into that directory with the
filename "key" (lowercase, no file extension)
