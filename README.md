TI Yocto BSP
===============================

TI Yocto manifest repository with Advantech layer

This repository is based on [ADVANTECH-Corp/adv-ti-yocto-bsp](https://github.com/ADVANTECH-Corp/adv-ti-yocto-bsp/tree/processor-sdk-03.01.00.06), and add additional EdgeSense feature.

BSP Source
----------

Create your own BSP folder first.
```
mkdir <BSP folder>
cd <BSP folder>
```

To get the latest version of Advantech meta layers, you can get without specific XML.
```
repo init -u git://github.com/ADVANTECH-Corp/adv-arm-yocto-bsp.git -b processor-sdk-03.01.00.06-EdgeSense
```

To get an official release version, you can assign the corresponding XML, e.g. version.xml.
```
repo init -u https://github.com/ADVANTECH-Corp/adv-arm-yocto-bsp.git -b processor-sdk-03.01.00.06-EdgeSense -m version.xml
```

Finally, pull down the BSP by running
```
repo sync
```

