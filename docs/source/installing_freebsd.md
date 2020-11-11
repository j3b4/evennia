# Installing on FreeBSD

This page describes how to install and run the Evennia server on a machine running [FreeBSD](https://www.freebsd.org/).

## Set up your system

This tutorial assumes that you have at a user account on the BSD machine who is a member of the _wheel_ group with 
access to the _su_ command to temporarily become the superuser. All commands should also work if simply run as root.
If you have _sudo_ then simply remember to prepend each example with the _sudo_ command.

```
$ cat file.txt
```
The `$` symbol is your prompt - do not include it when running commands.

## Prerequisites



This will create a new folder, called `evenv`, containing the new python executable.
Next, let's activate our new virtualenv. Every time you want to work on Evennia, you need to run the
following command:

```
$ source evenv/bin/activate
```
