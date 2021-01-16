# Coturn server for YunoHost

[![Integration level](https://dash.yunohost.org/integration/REPLACEBYYOURAPP.svg)](https://dash.yunohost.org/appci/app/REPLACEBYYOURAPP) ![](https://ci-apps.yunohost.org/ci/badges/REPLACEBYYOURAPP.status.svg) ![](https://ci-apps.yunohost.org/ci/badges/REPLACEBYYOURAPP.maintain.svg)  
[![Install Coturn with YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=REPLACEBYYOURAPP)

*[Lire ce readme en français.](./README_fr.md)*

> *This package allows you to install Coturn quickly and simply on a YunoHost server.  
If you don't have YunoHost, please consult [the guide](https://yunohost.org/#/install) to learn how to install it.*

## Overview
TURN and STUN server for VoIP
STUN (Session Traversal Utilities for NAT) and TURN (Traversal Using Relays around NAT) are protocols that can be used to provide NAT traversal for VoIP and WebRTC. This package provides a VoIP media traffic NAT traversal server and gateway. 

**Shipped version:** 4.5.1.1

## Configuration

How to configure this app: From an admin panel, a plain file with SSH, or any other way.

## Documentation

 * Official documentation: https://github.com/coturn/coturn/wiki
 * YunoHost documentation: If specific documentation is needed, feel free to contribute.

## YunoHost specific features

#### Multi-user support

Are LDAP and HTTP auth supported?
Can the app be used by multiple users?

#### Supported architectures

* x86-64 - [![Build Status](https://ci-apps.yunohost.org/ci/logs/REPLACEBYYOURAPP%20%28Apps%29.svg)](https://ci-apps.yunohost.org/ci/apps/REPLACEBYYOURAPP/)
* ARMv8-A - [![Build Status](https://ci-apps-arm.yunohost.org/ci/logs/REPLACEBYYOURAPP%20%28Apps%29.svg)](https://ci-apps-arm.yunohost.org/ci/apps/REPLACEBYYOURAPP/)

## Limitations

* Any known limitations.

## Additional information

* Other info you would like to add about this app.

**More info on the documentation page:**  
https://yunohost.org/packaging_apps

## Links

 * Report a bug: https://github.com/YunoHost-Apps/coturn_ynh/issues
 * Upstream app repository: https://github.com/coturn/coturn
 * YunoHost website: https://yunohost.org/

---

## Developer info

Please send your pull request to the [testing branch](https://github.com/YunoHost-Apps/coturn_ynh/tree/testing).

To try the testing branch, please proceed like that.
```
sudo yunohost app install https://github.com/YunoHost-Apps/coturn_ynh/tree/testing --debug
or
sudo yunohost app upgrade coturn -u https://github.com/YunoHost-Apps/coturn_ynh/tree/testing --debug
```

## Testing

For testing we can use Trickle-Ice testing tool. Go to trickle-ice page and enter following details.
```
STUN or TURN URI : turn:<YOUR_PUBLIC_IP_ADDRESS>:3478
TURN username: <YOUR_USERNAME>
TURN password: <YOUR_PASSWORD>
```
