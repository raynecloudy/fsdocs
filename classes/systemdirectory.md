---
icon: folder
---

# SystemDirectory

## Overview

The `SystemDirectory` class contains abstracted getters and setters for POSIX-defined attributes of a directory on the target file system. These include:

* atime (Last accessed)
* ctime (Creation date)
* Group (Coming soon)
* Mode (Permissions)
* mtime (Last modified)
* Path
* User (Coming soon)

> **Context**
>
> POSIX is a group of widely accepted standards to help preserve compatibility between operating systems.

> **Note**
>
> Due to a POSIX limitation, you cannot change the ctime of a directory.

## Properties

### accessed

Type: `Date`&#x20;

The `accessed` property returns when the directory was last accessed by a program.

### created

Type: `readonly Date`&#x20;

The `created` property returns when the directory was originally created.

### modified

Type: `Date`&#x20;

The `modified` property returns when the directory was last changed.

### path

Type: `string`&#x20;

The `path` property returns the full path to the directory.

When set, it moves the directory and its contents to the new location.

### permissions

Type: [`Permissions`](../interfaces/permissions.md)&#x20;

These are the permissions of the directory.
