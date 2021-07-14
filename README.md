<!--
N.B.: This README was automatically generated by https://github.com/YunoHost/apps/tree/master/tools/README-generator
It shall NOT be edited by hand.
-->

# Gemserv for YunoHost

[![Integration level](https://dash.yunohost.org/integration/gemserv.svg)](https://dash.yunohost.org/appci/app/gemserv) ![](https://ci-apps.yunohost.org/ci/badges/gemserv.status.svg) ![](https://ci-apps.yunohost.org/ci/badges/gemserv.maintain.svg)  
[![Install Gemserv with YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=gemserv)

*[Lire ce readme en français.](./README_fr.md)*

> *This package allows you to install Gemserv quickly and simply on a YunoHost server.
If you don't have YunoHost, please consult [the guide](https://yunohost.org/#/install) to learn how to install it.*

## Overview

A gemini server written in rust.

**Shipped version:** 0.4.5~ynh1



## Disclaimers / important information

* Other infos that people should be aware of, such as:
    * Redirect TCP/1965 port to the server
    * To add a gemini capsule, create a /etc/gemserv/config.d/example.toml 

```
[[server]]
hostname = "youdomain.org"
dir = "/path/to/serv/"
key = "/etc/yunohost/certs/youdomain.org/key.pem"
cert = "/etc/yunohost/certs/youdomain.org/crt.pem"
# index is optional but defaults to index.gemini. The server will serve files
# ending in gemini or gmi.
index = "index.gmi"
# lang is optional
lang = "en"
# cgi is optional bool
cgi = true
# cgipath is optional and only checked if cgi is true. It restricts cgi to only
# this directory.
cgipath = "/path/to/cgi-bin/"
# scgi is optional
scgi = { "/scgi" = "localhost:4000" }
# cgienv is optional
cgienv = { "GIT_PROJECT_ROOT" = "/srv/git" }
# usrdir is optional. it'll look in /home/usr/public_gemini
usrdir = true
# proxy is optional
# path is what comes after the hostname e.g. example.com/path
proxy = { path = "localhost:1966" }
# proxy_all is optional
# It will send all requests to the specified server. It also supports streamming.
proxy_all = localhost:1967
# redirect is optional
redirect = { "/redirect" = "/", "/newdomain" = "gemini://example.net" }
```
## Documentation and resources

* Upstream app code repository: https://codeberg.org/Valenoern/gemserv
* YunoHost documentation for this app: https://yunohost.org/app_gemserv
* Report a bug: https://github.com/YunoHost-Apps/gemserv_ynh/issues

## Developer info

Please send your pull request to the [testing branch](https://github.com/YunoHost-Apps/gemserv_ynh/tree/testing).

To try the testing branch, please proceed like that.
```
sudo yunohost app install https://github.com/YunoHost-Apps/gemserv_ynh/tree/testing --debug
or
sudo yunohost app upgrade gemserv -u https://github.com/YunoHost-Apps/gemserv_ynh/tree/testing --debug
```

**More info regarding app packaging:** https://yunohost.org/packaging_apps