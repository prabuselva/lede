# Description

This config can be used for compiling LEDE/OpenWRT for Xiaomi R3P Pro and Redmi AC2100 device

# Compilation

Command to compile,

```
# Command to download all dependencies first
$ make -j3 download V=s
# Command to compile the openWRT firmware 
$ make -j$(($(nproc) + 1)) V=s
```

# Flashing

Use the instructions from official openwrt website for both R3P and RM2100


# Initial Config for Xiaomi R3P

* Upon flashing, we need to open the /etc/wireless/l1profile.dat and change the "INDEX0=MT7603" to "INDEX0="MT7615"