# crypto-server
This repo contains scripts for automatic set-up of an Ubuntu server for running daemons for several cryptocurrencies.

# What it does
This script is meant to be run in shell through "./install_crypto_server" (Note that this file is being worked on and will be uploaded shortly.). It will create three hidden folders in the home folder: .crypto, .cryptoapps, and .cryptoscripts. In .crypto, the blockchains will be stored, with one (hidden) folder per cryptocurrency. In .cryptoapps, the repositories will be cloned and built, and so it will contain the daemon binaries. In .cryptoscripts, all of the scripts in this repo will be copied there, including the script runcryptoapps which can be used to run all of the daemons. Currently, all daemons, with the exception of Ethereum, will run in the background.  

# Supported cryptocurrencies
Currently supported cryptocurrencies are:

| Cryptocurrency  | Status| Source |
| --- | --- | --- |
| Bitcoin | Implemented | https://github.com/bitcoin/bitcoin.git |
| Bitcoin Cash | Implemented | https://github.com/Bitcoin-ABC/bitcoin-abc.git |
| Bitcoin Gold | Implemented | https://github.com/BTCGPU/BTCGPU.git |
| Litecoin | Implemented | https://github.com/litecoin-project/litecoin.git |
| Monero | Implemented | https://github.com/monero-project/monero.git |
| Ethereum | Implemented | https://github.com/ethereum/go-ethereum.git |
| Zcash | Planned | https://github.com/zcash/zcash.git |
| DigitalNote | Planned | https://github.com/DigitalNoteXDN/digitalnote.git |

# Supported OS's
This has only been tested on a clean and up-to-date Ubuntu Server 18.04.
