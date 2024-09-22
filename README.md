# Low-Cost-Preservation-Audio-Digitisation-with-Raspberry-Pi
This page provides information on low cost solutions for audio digitisation and preservation.  

The information listed here provides the basis for a workshop presented at the 55th International Association of Sound and Audiovisual Archives (IASA) conference, titled [Low Cost Preservation: Audio Digitisation with Raspberry Pi](https://iasavalencia24.sched.com/event/1f7qY/preservation-in-times-of-economic-crisis).

* [1. Raspberry Pi](#1-raspberry-pi)
* [2. HAT Options](#2-hat-options)
* [3. AES17 and IASA TC04 ADC Measurments](#3-aes17-and-iasa-tc04-adc-measurments)
* [4. "Cyberdeck"](#4-cyberdeck)
* [5. British Library Raspberry Pi Documentation](#5-british-library-raspberry-pi-documentation)

## 1. Raspberry Pi
A series of single board computers (SBC) developed by the [Raspberry Pi Foundation](https://www.raspberrypi.org/).  

Powered by ARM processors, the latest Raspberry Pi models (4 and 5) are available with 4GB or 8GB of RAM. They run [Raspberry Pi OS](https://www.raspberrypi.com/software/), a Debian-based Linux distribution, and are powerful enough to handle tasks such as running audio digitisation software.

## 2. HAT Options
Rasperry Pi hardware functionality can be expanded with [Hardware Attached on Top ("HAT")](https://www.raspberrypi.com/news/introducing-raspberry-pi-hats/) boards that mount directly onto the Pi board using the GPIO pins.  

There are a variety of quality Analogue-to-Digital Converter (ADC) and Digital-to-Digital (DDC) Converter HATs available for audio digitisation. For example: 

* [HiFiBerry](https://www.hifiberry.com)
* [Allo](https://www.allo.com)
* [JustBoom](https://shop.justboom.co/collections/raspberry-pi-audio-boards)


## 3. AES17 and IASA TC04 ADC Measurments
A suite of [AES17](https://www.aes.org/publications/standards/search.cfm?docID=21) (£) ADC measurments and their relative performance against the [IASA TC04, Key Digital Principles](https://www.iasa-web.org/tc04/key-digital-principles) for the [HifiBerry ADC+](/link), [Focusrite Scarlett](https://focusrite.com/products/scarlett-2i2) and [Prism Titan](https://beta.prismsound.com/products/titan/). 

* Download the [AES17 IASATC04 ADC Tests document](https://github.com/British-Library-Technical-Services/Low-Cost-Preservation-Audio-Digitisation-with-Raspberry-Pi/blob/2b49bbd1449693d2a5282cbe86c5c4fb27d1189e/AES17-IASATC04-ADC-Tests.pdf).

## 4. "Cyberdeck"
The concept for a low-cost, integrated and robust audio digitisation system was drawn from "cyberdeck" builds published by the open-source, hacker-developer community.  The main design for the prototype build presented here can be found at [the Raspberry Pi Recovery Kit](https://www.doscher.com/work-recovery-kit/).

## 4.1. Software
The Rasberry Pi's operating system is loaded via an SD card.  The most common OS available is Raspberry Pi OS (formally Raspian), maintained and distributed by the Raspberry Pi Foundation.  The Pi is capabale of running other popular Linux distributions such as [Ubuntu](https://ubuntu.com/download/raspberry-pi), [Fedora](https://docs.fedoraproject.org/en-US/quick-docs/raspberry-pi/) [Kali Linux](https://www.kali.org/docs/arm/raspberry-pi-4/).

A build of the Raspberry Pi OS, with pre-installed audio digitsation and digital preservation software, that can be flashed onto an SD card with software such as [Etcher](https://etcher.balena.io/) is available to download [here](/link _!pending_.

Most of the installed audio software is available to download directly in Raspberry Pi OS through [Pi-Apps](https://pi-apps.io/) (Desktop GUI) or [apt](https://en.wikipedia.org/wiki/APT_(software)) (Terminal).

#### 4.1.1 Audio Capture
* [Reaper 7](https://www.reaper.fm/) (£)
* [Audacity](https://www.audacityteam.org/)

#### 4.1.2. MiniDisc
* [QHiMDTransfer](https://wiki.physik.fu-berlin.de/linux-minidisc/doku.php?id=qhimdtransfer)
* [PlatinumMD](https://platinum-md.app/)

#### 4.1.3. ompact Disc
* [Brasero](https://wiki.gnome.org/Apps/Brasero)

#### 4.1.4. File Managment
* [VLC](https://www.videolan.org/)
* [FFMPEG](https://ffmpeg.org/)
* [MediaInfo](https://mediaarea.net/en/MediaInfo)
* [BWF MetaEdit](https://mediaarea.net/BWFMetaEdit)
* [KRename](https://apps.kde.org/krename/)

## 5. British Library Raspberry Pi Documentation
* [Raspberry Pi Audio Capture](https://british-library-technical-services.github.io/Documentation/docs/transfer_processes/raspberry_pi_audio_capture.html)
* [Timecoding in Reaper](https://british-library-technical-services.github.io/Documentation/docs/metadata/timecoding.html)
* [File Backup Service](https://github.com/British-Library-Technical-Services/file-backup-service) (Python 3.x code)