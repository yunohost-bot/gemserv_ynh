<!--
N.B.: This README was automatically generated by <https://github.com/YunoHost/apps/tree/master/tools/readme_generator>
It shall NOT be edited by hand.
-->

# Gemserv for YunoHost

[![Integration level](https://dash.yunohost.org/integration/gemserv.svg)](https://ci-apps.yunohost.org/ci/apps/gemserv/) ![Working status](https://ci-apps.yunohost.org/ci/badges/gemserv.status.svg) ![Maintenance status](https://ci-apps.yunohost.org/ci/badges/gemserv.maintain.svg)

[![Install Gemserv with YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=gemserv)

*[Read this README in other languages.](./ALL_README.md)*

> *This package allows you to install Gemserv quickly and simply on a YunoHost server.*  
> *If you don't have YunoHost, please consult [the guide](https://yunohost.org/install) to learn how to install it.*

## Overview

A gemini server written in rust.

### Features

- Vhosts
- CGI
- User directories
- Reverse proxy
- Redirect
- SCGI
- Reload config on SIGHUP


**Shipped version:** 0.6.6~ynh8
## Documentation and resources

- Official app website: <https://git.sr.ht/~int80h/gemserv/>
- Upstream app code repository: <https://git.sr.ht/~int80h/gemserv>
- YunoHost Store: <https://apps.yunohost.org/app/gemserv>
- Report a bug: <https://github.com/YunoHost-Apps/gemserv_ynh/issues>

## Developer info

Please send your pull request to the [`testing` branch](https://github.com/YunoHost-Apps/gemserv_ynh/tree/testing).

To try the `testing` branch, please proceed like that:

```bash
sudo yunohost app install https://github.com/YunoHost-Apps/gemserv_ynh/tree/testing --debug
or
sudo yunohost app upgrade gemserv -u https://github.com/YunoHost-Apps/gemserv_ynh/tree/testing --debug
```

**More info regarding app packaging:** <https://yunohost.org/packaging_apps>
