<!--
N.B.: This README was automatically generated by https://github.com/YunoHost/apps/tree/master/tools/README-generator
It shall NOT be edited by hand.
-->

# Misskey for YunoHost

[![Integration level](https://dash.yunohost.org/integration/misskey.svg)](https://dash.yunohost.org/appci/app/misskey) ![](https://ci-apps.yunohost.org/ci/badges/misskey.status.svg) ![](https://ci-apps.yunohost.org/ci/badges/misskey.maintain.svg)  
[![Install Misskey with YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=misskey)

*[Lire ce readme en français.](./README_fr.md)*

> *This package allows you to install Misskey quickly and simply on a YunoHost server.
If you don't have YunoHost, please consult [the guide](https://yunohost.org/#/install) to learn how to install it.*

## Overview

Misskey is a decentralized microblogging platform. Since it exists within the Fediverse (a universe where various social media platforms are organized), it is mutually linked with other social media platforms.


**Shipped version:** 12.96.1~ynh1



## Screenshots

![](./doc/screenshots/screenshot.jpg)

## Disclaimers / important information

### Important points to read before installing

- *Misskey* require a dedicated root domain, eg. `misskey.domain.tld`
- *Misskey* can take quite some time to install (more then 30 minutes). So take out some time and grab yourself a coffee.
- If installing from command line use of screen is rerecorded to avoid disconnection. See below.
- After installation, first page can take time to load and may show timeout error. Give it time to make itself ready for you. Refresh page after 2-3 minutes.
- The first account created will be an admin user and will have all the admin rights.

Using screen in case of disconnects

``` 
sudo apt-get install screen
screen
sudo yunohost app install https://github.com/YunoHost-Apps/misskey_ynh.git
```
Recover after disconnect:
```
screen -d
screen -r
```

## Documentation and resources

* Official app website: https://join.misskey.page
* Upstream app code repository: https://github.com/misskey-dev/misskey
* YunoHost documentation for this app: https://yunohost.org/app_misskey
* Report a bug: https://github.com/YunoHost-Apps/misskey_ynh/issues

## Developer info

Please send your pull request to the [testing branch](https://github.com/YunoHost-Apps/misskey_ynh/tree/testing).

To try the testing branch, please proceed like that.
```
sudo yunohost app install https://github.com/YunoHost-Apps/misskey_ynh/tree/testing --debug
or
sudo yunohost app upgrade misskey -u https://github.com/YunoHost-Apps/misskey_ynh/tree/testing --debug
```

**More info regarding app packaging:** https://yunohost.org/packaging_apps