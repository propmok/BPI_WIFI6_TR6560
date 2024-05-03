# BPI WIFI6 TR6560
openwrt source code for tr6560 and custom sysupgrade.bin


Banana Pi WIFI 6 TR6560 router

when compiling the source code from https://github.com/BPI-SINOVOIP/THG6500-TAX2-OPENWRT-BSP I kept running into an issue where make would fail telling me ../bin/ was not a directory.
workaround for this issue was to run make, let it fail, check to see if <build folder>/bin/ exists, if not create it, then locate <build folder>/bin/targets/tr6560/generic/TR6560-bootimage.bin and copy to <build folder>/bin/

this is only required if you need the fullimage.bin because sysupgrade.bin compiles fine

I have included my compiled sysupgrade.bin file with wireguard, adblock and wake on lan options added.
