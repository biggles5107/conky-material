# conky-material

A dynamic conky script using Material Design colors.

![conky-material](http://i.imgur.com/91VsSxm.png)

## Notable Features

* Network stats change based on wired, wireless, or no connection
* Pulls useful GPU stats from `nvidia-smi` (sorry, AMD/ATI users)
* Dynamically adds disk usage and I/O for removable disks (not sure if this works under KDE)

## Installation

### Prerequisites

* [conky 1.9](https://github.com/brndnmtthws/conky/releases/tag/1.9.0) (1.10 will not work because it uses the new Lua syntax)
* [Noto Sans](https://www.google.com/get/noto/)
* [Source Code Pro](https://github.com/adobe-fonts/source-code-pro/releases/latest)

### Instructions

Copy all files (except this README) to your home folder.

Edit to your heart's content. Disk partitions, network interfaces, and sensors will probably be different for you; make sure to edit accordingly. Adding disk partitions (e.g., if you have `/usr` on a separate partition) is as easy as adding a single line:

```
${template0 /usr}
```

That's it! To add disk I/O (e.g., if `/usr` is mounted on `/dev/sda3`), just add another line like so:

```
${template2 sda3}
```
