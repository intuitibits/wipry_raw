# wipry_raw

A command-line utility to dump spectral data from an [Oscium WiPry Clarity](https://oscium.com/products/wipry-clarity/) spectrum analyzer.

```
Usage: wipry_raw [options]
Options:
  -l, --list-ranges    List supported ranges.
  -r, --range RANGE    Use RANGE.
  -h, --help           Print this message and exit.
```

### Requirements

* Requires [libusb](https://github.com/libusb/libusb).

### Installation

```
# Install pre-requisites
sudo apt update
sudo apt install libusb-1.0-0

# Install wipry_raw
unzip wipry_raw-1.0.0_arm64.zip
sudo mv wipry_raw /usr/bin/

# Configure passwordless sudo
echo "%sudo ALL = (root) NOPASSWD: /usr/bin/wipry_raw" | sudo tee /etc/sudoers.d/wipry_raw
sudo chmod -x /etc/sudoers.d/wipry_raw
```
---

To report any issues please contact Intuitibits Support by emailing support@intuitibits.com.

_Oscium and WiPry are all registered trademarks of Dechnia, LLC._
