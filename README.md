# Electrum - Lightweight Bitcoin client [Official site](https://electrum-btc.org)_

```
Licence: MIT Licence
Author: Thomas Voegtlin
Language: Python (>= 3.8)

```


## Getting started

_(If you've come here looking to simply run Electrum,
[you may download Electrum wallet here](https://electrum-btc.org/download).)_

Electrum itself is pure Python, and so are most of the required dependencies,
but not everything. The following sections describe how to run from source, but here
is a TL;DR:

```
$ sudo apt-get install libsecp256k1-dev
$ python3 -m pip install --user ".[gui,crypto]"
```

### Not pure-python dependencies

If you want to use the Qt interface, install the Qt dependencies:
```
$ sudo apt-get install python3-pyqt5
```

For elliptic curve operations,
[libsecp256k1](https://github.com/bitcoin-core/secp256k1)
is a required dependency:
```
$ sudo apt-get install libsecp256k1-dev
```

Alternatively, when running from a cloned repository, a script is provided to build
libsecp256k1 yourself:
```
$ sudo apt-get install automake libtool
$ ./contrib/make_libsecp256k1.sh
```

Due to the need for fast symmetric ciphers,
[cryptography](https://github.com/pyca/cryptography) is required.
Install from your package manager (or from pip):
```
$ sudo apt-get install python3-cryptography
```
