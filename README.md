Ansible io.js Role
=========

[![Build Status](https://secure.travis-ci.org/martinmicunda/ansible-role-iojs.png)](http://travis-ci.org/martinmicunda/ansible-role-iojs) [![Ansible Galaxy](http://img.shields.io/badge/galaxy-martinmicunda.iojs-blue.svg)](https://galaxy.ansible.com/list#/roles/1700) [![Platforms](http://img.shields.io/badge/platforms-ubuntu-orange.svg)](#)

An ansible role for installing io.js and NPM.

Installation
------------
This role requires at least Ansible `v1.7.0`. To install it, run:

```bash
$ ansible-galaxy install martinmicunda.iojs
```

Requirements
------------

Currently it's been developed for, and tested on `Ubuntu`.

Role Variables
--------------

List of default variables available in the inventory:

| Name                    | Default   | Description      |
| ----------------------- | --------- | ---------------- |
| iojs_version            | 1.3.0     | io.js version  |
| iojs_filename           | iojs-v{{ iojs_version }}-linux-x64 | io.js filename |

Example Playbook
----------------

Add `martinmicunda.iojs` to your roles and overwrite default vars (optional) in your playbook file.

    - hosts: all
      roles:
         - role: martinmicunda.iojs
      vars:
         - iojs_version: "1.4.0"  

License
-------

    The MIT License
    
    Copyright (c) 2015 Martin Micunda  

    Permission is hereby granted, free of charge, to any person obtaining a copy
    of this software and associated documentation files (the "Software"), to deal
    in the Software without restriction, including without limitation the rights
    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
    copies of the Software, and to permit persons to whom the Software is
    furnished to do so, subject to the following conditions:
    
    The above copyright notice and this permission notice shall be included in
    all copies or substantial portions of the Software.
    
    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
    THE SOFTWARE.
