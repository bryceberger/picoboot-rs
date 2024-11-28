# picoboot-rs &ensp; [![github]](https://github.com/NotQuiteApex/picoboot-rs) &ensp; [![crates-io]](https://crates.io/crates/picoboot-rs) &ensp; [![docs-rs]](https://docs.rs/picoboot-rs)
A crate for connecting to and communicating with a Raspberry Pi microcontroller in BOOTSEL mode over USB!

[github]: https://img.shields.io/badge/github-8da0cb?style=for-the-badge&labelColor=555555&logo=github
[crates-io]: https://img.shields.io/badge/crates.io-fc8d62?style=for-the-badge&labelColor=555555&logo=rust
[docs-rs]: https://img.shields.io/badge/docs.rs-66c2a5?style=for-the-badge&labelColor=555555&logo=docs.rs

## Notes
When using this crate, the underlying dependencies will be downloaded and installed automatically, however further configuration for USB devices on the host machine may be required.

- When running on Linux or macOS, you may need to add some additional udev rules to allow the PICOBOOT interface to be usable by a userspace program. These udev rules can be found [here](https://github.com/raspberrypi/picotool/blob/master/udev/99-picotool.rules).
- When running on Windows, you may need to install a libusb compatible driver for the PICOBOOT interface. This driver can be installed by [Zadig](https://zadig.akeo.ie/). Simply plug in the Pico device while holding the BOOTSEL button, and install any of the listed drivers for the RP2 Boot device in Zadig.

## License
The contents of this repository are dual-licensed under the _MIT OR Apache 2.0_
License. That means you can choose either the MIT license or the Apache 2.0
license when you re-use this code. See [`LICENSE-MIT`](./LICENSE-MIT) or
[`LICENSE-APACHE`](./LICENSE-APACHE) for more information on each specific
license. Our Apache 2.0 notices can be found in [`NOTICE`](./NOTICE).

Unless you explicitly state otherwise, any contribution intentionally submitted
for inclusion in the work by you, as defined in the Apache-2.0 license, shall be
dual licensed as above, without any additional terms or conditions.

## Acknowledgements
* [rp-rs Developer Group](https://github.com/rp-rs)
* Raspberry Pi microcontroller datasheets for [RP2040](https://datasheets.raspberrypi.com/rp2040/rp2040-datasheet.pdf) and [RP2350](https://datasheets.raspberrypi.com/rp2350/rp2350-datasheet.pdf)
* [Raspberry Pi](https://raspberrypi.org), [Pico SDK](https://github.com/raspberrypi/pico-sdk), and [Picotool](https://github.com/raspberrypi/picotool)
* This project and the PICOBOOT interface provided by Raspberry Pi microcontrollers are NOT affiliated with the [Nintendo GameCube hardware hack of the same name](https://github.com/webhdx/PicoBoot).
