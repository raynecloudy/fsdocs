---
icon: lock-keyhole
---

# Permissions

## Overview

The `Permissions` interface defines properties that follow the POSIX standard for file and directory permissions.

## Properties

### everyone

Type: [`RWX`](interfaces/rwx.md)&#x20;

The permissions for everyone except the owner and group of the file/directory.

### group

Type: [`RWX`](interfaces/rwx.md)

The permissions for the group of the file/directory.

### user

Type: [`RWX`](interfaces/rwx.md)&#x20;

The permissions for the owner of the file/directory.
