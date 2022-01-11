# GD32 Duino-Coin Miner

## Description

Contains the firmware and miner software for minign [DUCO (Duino-Coin)](https://github.com/revoxhere/duino-coin) on GigaDevice GD32 chips. 

## Supported boards

* GD32E503C-START (GD32E503CET6)
* more to come

## Compiling the firmware

Use the [PlatformIO]() build system to compile the firmware. You also see the steps at related projects like [here](https://github.com/CommunityGD32Cores/gd32-pio-projects#importing-examples).

## Performance

| Device        | Hashrat       | Profit (ᕲ/day)  |
| ------------- |:-------------:| -----:|
| GD32E503CE    | 42.9 kH/s     | to be measured |

## Mining

Start the `GD32_Miner.py` Python script with at least Python version 3. 

At the first run, you will be prompted for the DUCO wallet username to send coins to.  

Settings like the COM port on which the GD32 device is available will be auto-deteced at the first start and written into the `Duino-Coin GD32 Miner 2.75/Settings.cfg` file.

![miner](mining.png)

## Notes

It is normal to get the first few shares REJECTED as they're on a too low difficulty. The Kolka balancing will kick in shortly.