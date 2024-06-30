# kaspad-stratum

FreeBSD port of `kaspad-startum` from https://github.com/fungibilly/kaspad-stratum.

## Installation
- Install `pkg install rust`
- Checkout repository and `cd` to the folder
- The `cd` into the port directory `cd freebsd/port`
- Run `make install`

## Usage
To start, simply run
```commandline
kaspad-stratum -m <KASPA_WALLET_ADDRESS> -r <KASPAD_RPC_URL>
```
This will start a stratum server at `127.0.0.1:6969`.

Additional options:
- `-s <IP:PORT>`:  change the stratum server address
- `-e <EXTRA_DATA>`: change the extra data
- `-d`: show debug output

## Known Limitations

Unfortunately this server was written before ASIC's where made available 
for Kaspa mining, therefore it lacks proper support for ASIC's.

If yo uare a rust developer and are familiar with the changes needed to
make this software ASIC compatable, please open a PR with your contributions.

