# Xdebug Toggler pour MACOS

![](screenshot.png "Example")

Le script permet via `on|true` et `off|false` d'activer automatiquement [Xdebug][xdebug] si l'installation des différentes version de PHP on était faites [sphp](https://github.com/conradkleinespel/sphp-osx) en suivant les tutos suivant :
* [Tuto-1](http://getgrav.org/blog/mac-os-x-apache-setup-multiple-php-versions)
* [Tuto-2](http://getgrav.org/blog/mac-os-x-apache-setup-mysql-vhost-apc)

## Installation

```
curl -L https://raw.githubusercontent.com/gemy-athena/xdebug-osx/master/debug > /usr/local/bin/xdebug-toggle
```

## Rendre `xdebug-toggle` éxécutable

```
chmod +x /usr/local/bin/debug
```

## Utilisation
```
debug                                # donne le status courant
debug on                             # active xdebug
debug true                           # active xdebug
debug off                            # désactive xdebug
debug false                          # désactive xdebug
debug on|off --no-server-restart     # toggles xdebug sans redémarrer apache ou php-fpm
debug true|false --no-server-restart # toggles xdebug sans redémarrer apache ou php-fpm
```

## License
[LICENSE](LICENSE)

[xdebug]: http://xdebug.org/
[brew]: http://brew.sh/
[grav]: http://getgrav.org/
[tutorial-1]: http://getgrav.org/blog/mac-os-x-apache-setup-multiple-php-versions
[tutorial-2]: http://getgrav.org/blog/mac-os-x-apache-setup-mysql-vhost-apc
[sphp]: https://github.com/conradkleinespel/sphp-osx
