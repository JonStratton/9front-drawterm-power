# 9front-drawterm-power
Fork of 9front's drawterm to try to get it to build on PowerMacs running OS X 10.4

http://git.9front.org/plan9front/drawterm/HEAD/info.html

Currently, only OS X X11 version works (ie not Cocoa). So you need X11 to run.

## To Build

CONF=osx-x11 make

## Changes
# kern/qio.c
Removed 'typedef struct Queue   Queue;'

# libmemdraw/warp.c
s/Σ/sigma/g
s/Δ/delta/g
s/₀/zero/g
s/₁/one/g
s/₂/two/g
s/₃/three/g

# posix-power/*
Pulled from "posix-power" from http://git.9front.org/git/plan9front/drawterm/789b8fe40e156ad0252230b13dd4ada96f3eed8b/snap.tar.gz

# Makefile
Pointed at posix-power.
