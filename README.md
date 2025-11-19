<p align="center"><br>
<a href="https://makeapullrequest.com"><img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg"></a>
<a href="https://dortania.github.io/OpenCore-Install-Guide/"><img src="https://img.shields.io/badge/fully-hackintosh-white"></a>
<br><p>

<h3 align="center">
run macOS on your ASUS TUF FX series laptop(s)! (you can extend compatibility with little to no edits)!
</h3>

<h1 align="center">
showcase (screenshots)
</h1>

![screenshots](./showcase.jpg)

> [!WARNING]  
> don't forget to map your USB ports, otherwise USB compatibility might crap out, and your ports could be out of wack! you can check out USBMap to do such.

> [!TIP]
> you can use a newer version of macOS on this EFI build! just make sure to also update OpenCore as it is quite outdated since then. otherwise, everything should be all right!

## table of contents

- [information](#information)
- [compatibility](#compatibility)
- [how to use](#how-to-use)
- [donating](#donating)
- [contributing](#contributing)
- [reporting issues](#reporting-issues)
- [credits](#credits)
- [license](#license)

## information

| version info       | data                                           |
| --------------- | ------------------------------------------------ |
| OpenCore             | 0.9.8             |
| macOS tested            | tested w/ Monterey           |
| status           | works quite well lol      

## compatibility

- ✅ - works and tested
- ⚠️ - work in progress by the OpenCore team
- ❌ - broken, possible fix
- ⛔ - impossible to fix

| part       | model/data                                           | status             | other info             |
| --------------- | ------------------------------------------------ | --------------- | ---------------          |
| `CPU`             | Intel Core i5-8300H (Coffee Lake)             | ✅             | works |
| `GPU`             | NVIDIA Mobile 1050Ti                        | ⛔             | no macOS drivers for NVIDIA since High Sierra |
| `eGPU`            | Intel Graphics UHD 630                       | ✅             | works with acceleration |
| `audio`           | Realtek ALC233                                | ✅             | works |
| `ethernet`        | Realtek RTL8168/8111                         | ✅             | works |
| `Wi-Fi`          | Intel Wireless-AC 9560                  | ⚠️ | works but experimental, intel wifi is quirky | 
| `Bluetooth`      | Intel Bluetooth                              | ⚠️ | works, but same as for Intel WiFi. experimental. | 
| `touchpad`       | Trackpad ELAN1200 I2C-HID                    | ✅             | works. if you get weird feedback, make sure to check your force touch settings! | 
| `keyboard`       | Keyboard PS2                                 | ⚠️             | works, but backlight and function keys are crapped out | 
| `battery`        | Asus Default Battery                         | ✅             | works | 
| `webcam`         | USB2.0 HD UVC WebCam Internal                                              | ✅             | works | 
| `microphone`     | Realtek micwopon                                            | ✅             | works | 
| `USB ports`     | 3 USB 2.0, 2 USB 3.1                                         | ✅             | works, don't forget to map your USB ports | 
| `fans`           | 2 Fans                                              | ⚠️             | works, but no accurate fan readings |

## how to use
if you've never done this, please check out [Dortania's guide](https://dortania.github.io/OpenCore-Install-Guide/)! this is the most accurate place for information.

once done, you'll need to start by making a bootable USB key with the macOS installer, you can do such by following the guide, and when the time comes to import an EFI folder, get mine from GitHub: either using git clone or the releases (source will be more up to date), and then pasting the EFI on your USB key.

you can then boot and try to install, and enjoy!

## donating
this is free and open source software! I don't expect any kind of funding or donations, but they are always appreciated as this is work that's definitly free will and getting some donation helps keep up the good work! Your donation will only and ONLY be used towards improving our software in the [organization's mission](https://hcb.hackclub.com/lonersoft/donations). we are fully transparent and open source with our finances!

[you can donate here](https://hcb.hackclub.com/donations/start/lonersoft) and [check our finances here](https://hcb.hackclub.com/lonersoft)!

## contributing
contributions of any kinds are accepted. you can, for example, add compatibility for other laptops of this similar kind and publish your EFI suggestions in this repo! to get started, clone the repository, and open it in a PLIST editor:

```sh
git clone https://github.com/lonersoft/ASUS-TUF-FX-Hackintosh.git
cd "ASUS-TUF-FX-Hackintosh"
```

you may then request your modifications via a PR.

## reporting issues
this is a community project, and your help is very much appreciated! if you notice anything wrong during your usage of this software, please report it to the [GitHub issues page](https://github.com/lonersoft/ASUS-TUF-FX-Hackintosh/issues/)!

## credits
many thanks to these who without them, the project may have never seen the light of day (or it would just have sucked):

- [Dortania](https://dortania.github.io/) - main hackintosh guide, the best reference by today's standards for making hackintosh

- [Acidathera](https://github.com/acidanthera) - OpenCore and main kexts

- [doanhxd](https://github.com/doanhxd/Asus-TUF-Gaming-FX505GE-Hackintosh) - main reference as for the hackintosh EFI!

- [RehabMan](https://github.com/RehabMan) - different ACPI patches that helped very well!

- [DotCube123](https://github.com/DotCube123/Asus-Tuf-Gaming-FX705GE-Hackintosh) - used this as a reference for fixing stuff w/ newer versions of macOS!

and probably some others I forgotten.. sorry in advance, but thanks for being here!

## license
this project is licensed under the MIT License which you may check [here](https://github.com/lonersoft/ASUS-TUF-FX-Hackintosh/blob/master/LICENSE/).
<br>if you have any questions about this project or inquieries, please reach us at [team@loners.software](mailto:team@loners.software).
