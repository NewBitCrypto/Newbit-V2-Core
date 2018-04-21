NewBit Cryptocurrency

#### Table of Contents

* [Features](#features)
* [Usage](#usage)
  * [Downloading & Installing](#1-downloading--installing)
  * [Configuration](#2-configuration)

  * [Forknote](#2-forknote)
* [Coins Using This Software](#coins-using-this-software)
* [Community / Support](#community--support)
* [Contributing](#contributing)

#### Features

* Cryptonote source code creation, based on:
   * Bytecoin code (latest version)
* Single command code and binaries update
* Simple update for existing code
* Compile for
  * Windows (tested on 8.1)
  * Ubuntu (tested on 14.04)
  * Mac OS X (tested on Yosemite)

Usage
===

#### 1) Downloading & Installing

Clone the repository:

```bash
	git clone https://github.com/forknote/cryptonote-generator.git generator
	cd generator
```

Install dependencies:

* Windows - [follow this instructions](https://github.com/dashcoin/cryptonote-generator/blob/master/docs/windows-requirements-install.md)
* Linux / Mac OS X
```
bash install_dependencies.sh
```

#### 3) Generate coin

The file `config.json` is used by default but a file can be specified using the `-f file` command argument, for example:

```bash
	bash generator.sh -f [CONFIG_FILE] [-c COMPILE_OPTIONS]
```

By default, the cryptonote generator is not using multithread. I strongly recommend to use this arguments, if you are not building on a on VPS with no swap defined

###### Windows:
```bash
	bash generator.sh -f config_example.json -c '/maxcpucount:3'
```

###### Linux / Mac OS X (Cmake 2.8.x):
```bash
	bash generator.sh -f config_example.json -c '-j3'
```

To generate NewBit:
```
	git clone https://github.com/NewBitCrypto/cryptonote-generator.git generator && cd generator
	bash install_dependencies.sh && bash generator.sh -f configs/bytecoin-v2/config_example.json
```



### Community / Support

* IRC (freenode)
  * Support / general / development discussion join #dashcoin: [https://webchat.freenode.net/?channels=#dashcoin](https://webchat.freenode.net/?channels=#dashcoin)
* [CryptoNote Forum](https://forum.cryptonote.org/)


#### Projects Using This Software

* [Dashcoin](https://bitcointalk.org/index.php?topic=1020627.0)
* [Forknote](https://bitcointalk.org/index.php?topic=1079306.0)


#### Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

Extensions must be located in *extensions* folder.


Donations
---------
* BTC: `1EYiA8o1KsDZxMHXvptxXyaVwuhTVNBMFp`
* DSH: <sup><sub>`D3z2DDWygoZU4NniCNa4oMjjKi45dC2KHUWUyD1RZ1pfgnRgcHdfLVQgh5gmRv4jwEjCX5LoLERAf5PbjLS43Rkd8vFUM1m`</sup></sub>
* BCN: <sup><sub>`21YR5mw5BF2ah3yVE3kbhkjDwvuv21VR6D7hnpm4zHveDsvq5WEwyTxXLXNwtU5K4Pen89ZZzJ81fB3vxHABEUJCAhxXz2v`</sup></sub>
* XMR: <sup><sub>`47LEJyhCgNFcoz6U8x7tUk6LEHe38NobAfn4ou8d588jY5nddvgEANLMMcwxsbfbkJRw4xPwcG583Gq189hjusShEyk9FXz`</sup></sub>

*Donate XMR if you want to XMR version to be developed*

Additional credits
------------------
* [piotaak](https://github.com/piotaak) (tests for cryptonotecoin-core extension)

License
-------
Released under the GNU General Public License v2

http://www.gnu.org/licenses/gpl-2.0.html
