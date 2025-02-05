# itconfigPI

Optimized Deluge settings for Raspberry Pi and other low-power systems to prevent CPU overload rendering other services unusable.

## Overview
This project provides a fine-tuned configuration for Deluge on Raspberry Pi & other low power systems, ensuring efficient performance while avoiding excessive resource usage and preventing other services from being overloaded due to excessive read/write operations.

## Features
- Optimized cache settings to reduce disk I/O.
- Limited concurrent connections to prevent CPU and RAM overload.
- Tweaked queue and bandwidth settings for a balanced download experience.
- Configured to minimize the impact on other running services by reducing excessive read/write operations while trying to not over limit Deluge performance.

## Installation
1. Clone this repository:
   ```sh
   git clone https://github.com/seedboxer/itconfigPI.git

   cd itconfigPI

   cp core.conf ~/.config/deluge/

systemctl restart deluged

## Compatibility

- Designed for Raspberry Pi (tested on Raspberry Pi 3, 4, and 5) as well as other low-power systems
- Works with Deluge 2.x.

## Notes

- Adjust final settings as needed based on your network speed and storage setup.
- Ensure Deluge is stopped before modifying core.conf to avoid corruption.

License

This project is released under the MIT License.
