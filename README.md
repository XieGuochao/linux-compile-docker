# Linux Compile Docker

## Motivation

I develop this project because I find lots of trouble when I try to compile 
an old kernel on my server running on the latest Ubuntu. More specifically,
I will need an old `gcc` and related tools to compile the old kernel. 
Otherwise, there are lots of security warning and issues fail my compilation.

Even more, I am trying to use my MacBook M1 chip to cross compile the x86-64
kernel because my new MacBook is super fast! Let's see if I can succeed!

## Organization

This project is organized with multiple folders, each is responsible for one 
kernel version (major or minor version). Users need to mount and unmount kernel
and kernel output folders to the container and use the container's environment
for compilation.

## How to use

Run `docker run --rm -it -v {Linux source code}:/linux -v {Linux output}:/linux-output linux-compile-docker`.