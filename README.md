# Let's Encrypt Plugin for cPanel

[![Codacy](https://img.shields.io/codacy/grade/f07779f4de8f44b7a67f88f0954a2371/master.svg?style=flat-square)](https://www.codacy.com/app/CyanDarkInc/LetsEncrypt-cPanel?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=CyanDarkInc/LetsEncrypt-cPanel&amp;utm_campaign=Badge_Grade)

This is a cPanel/WHM plugin for the [Let's Encrypt](https://letsencrypt.org/) client. This plugin uses Perl and the WHM API, and requires a server running cPanel and WHM on it.

Support for service SSL certificates has been recently added, and is considered to be in beta. Please report any issues you find so that we may address them.

### Version
Version 1.0

### Requirements

- CentOS 6/7
- cPanel 11.48 or Later

### Installation

```
/usr/local/cpanel/3rdparty/bin/git clone https://github.com/CyanDarkInc/LetsEncrypt-cPanel.git
cd letsencrypt-cpanel
./install.sh
```

If everything goes well, you will see a new icon in the `WHM >> Plugins` section. Existing certificates will be shown, and you will be able to register new SSL certificates for domains on the server that do not yet have SSL associated with it.

Any SSL certificates added will automatically attempt renewal. You should not need to manually renew the certificates.

### Upgrading
	
```
cd letsencrypt-cpanel
/usr/local/cpanel/3rdparty/bin/git pull
./upgrade.sh
```

### Uninstall
	
```
cd letsencrypt-cpanel
./uninstall.sh
```
