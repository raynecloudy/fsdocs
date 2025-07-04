---
icon: file
---

# SystemFile

## Overview

The `SystemFile` class contains abstracted getters and setters for POSIX-defined attributes of a file on the target file system. These include:

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
> Due to a POSIX limitation, you cannot change the ctime of a file.

## Properties

### accessed

Type: `Date`&#x20;

The `accessed` property returns when the file was last accessed by a program.

### content

Type: `string`&#x20;

The `content` property returns the current content in the file located at the value of the `SystemFile`'s `path`.

When set, it overwrites the current content of the file with the provided string.

### created

Type: `readonly Date`&#x20;

The `created` property returns when the file was originally created.

### modified

Type: `Date`&#x20;

The `modified` property returns when the content of the file was last changed.

### path

Type: `string`&#x20;

The `path` property returns the full path to the file.

When set, it moves the file to the new location.

### permissions

Type: [`Permissions`](../interfaces/permissions.md)&#x20;

These are the permissions of the file.
