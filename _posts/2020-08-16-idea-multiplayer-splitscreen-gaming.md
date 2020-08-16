---
layout: post
title:  "Idea: Multiplayer Split-Screen Console Gaming"
date:   2020-08-16 14:00:00 -0700
tags: ideas social gaming
---
In the days before online multiplayer video games, people used to get together
around a single television and play split-screen multiplayer games. If one
wanted to play these old multiplayer games between houses, one approach would
be to connect the composite output to an RF modulator/CATV amplifier capable
of generating a signal in the amateur bands, then connect the modulator to
an antenna. It might be necessary to leave the audio portion disconnected if
the game didn't allow the music to be turned off; however then the audio
carrier could be used as a duplex mode voice chat.

The controller would be the complicated part. However it might be possible to
use a Part 15 bidirectional serial radio module connected to a high-gain
directional antenna. Part 15 would make things a bit simpler since there would
be no need to identify. It would likely be necessary to develop a bit of
interoperabilty code to translate the data output by the controller/console to
a form that could be sent by the serial module, as well as a bit of hardware
that could connect the controller and console to the serial modules. This could
probably be accomplished with something like an arduino and provide for minimal
latency between performing an action using the controller and having the console
respond.
