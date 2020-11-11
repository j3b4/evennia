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

# Install Python

`$ sudo pkg install python`

```
Note that some standard Python modules are provided as separate ports
as they require additional dependencies. They are available as:

py37-gdbm       databases/py-gdbm@py37
py37-sqlite3    databases/py-sqlite3@py37
py37-tkinter    x11-toolkits/py-tkinter@py37
```
Install the first two but I don't think you'll need x11 for a server.

`$ sudo pkg install py37-gdbm py37-sqlite3`

`sudo pkg install py37-pip`

## Install GIT

`sudo pkg install git`

## Install pip
 `sudo pkg install py37-pip`

## Install virtualenv
`sudo pip install virtualenv`

## Make a folder for Evennia
```
$ mkdir  evdev
$ cd evdev
```
### Clone Evennia
`git clone https://github.com/evennia/evennia.git`

### Create the virtual env

virtualenv evenv

This will create a new folder, called `evenv`, containing the new python executable.
Next, let's activate our new virtualenv. Every time you want to work on Evennia, you need to run the
following command:

```
$ source evenv/bin/activate
```
