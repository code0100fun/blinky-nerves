# Blinky

Blinking LED example for Beagle Bone Black.

## Development

Install Dependencies:

```
$ mix deps.get
```

Install Bakeware:

```
$ ruby -e "$(curl -fsSL https://bakeware.herokuapp.com/bake/install)"
```

**Valid targets are bbb, rpi2, rpi, or all**

Get the system

```
$ bake system get --target bbb
```

Get the toolchain

```
$ bake toolchain get --target bbb
```

## Buiding Firmware

**Valid targets are bbb, rpi2, rpi, or all**

```
$ bake firmware --target bbb
```

## Burn to SD Card

On OSX:

```
$ sudo fwup -a -i _images/blinky-bbb.fw -t complete
```

## Connecting

With FTDI (3.3v):

```
$ screen /dev/tty.usbserial-A400BZH8 115200
```

**Note: This will not work in a tmux session!**

**Note: To disconnect use [Ctrl]-A K**

