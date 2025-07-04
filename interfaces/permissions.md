---
icon: lock-keyhole
---

# Permissions

## Overview

The `Permissions` interface defines properties that follow the POSIX standard for file and directory permissions.

## Properties

### code

Type: `number`

This is the "mode" of the file/directory. It's a three-digit number that defines permissions for everyone, group, and user. Learn more about permission modes [here](https://www.linuxfoundation.org/blog/blog/classic-sysadmin-understanding-linux-file-permissions#h-using-binary-references-to-set-permissions).

### everyone

Type: [`RWX`](rwx.md)

The permissions for everyone except the owner and group of the file/directory.

### group

Type: [`RWX`](rwx.md)

The permissions for the group of the file/directory.

### user

Type: [`RWX`](rwx.md)

The permissions for the owner of the file/directory.
