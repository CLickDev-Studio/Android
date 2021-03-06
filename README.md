﻿﻿﻿ClickProject Oreo
===========
ClickProject just an AOSP ROM with some extra features,which provide by **OpenSource Projects**,Some builds was optimized for each devices or localized.

Credits
-------
* [**JDCTeam**](https://github.com/AOSP-JF-MM)
* [**DirtyUnicorns**](https://github.com/DirtyUnicorns)
* [**TeamSubstratum (Theme Engine)**](https://github.com/Substratum)
* [**LineageOS/Cyanogenmod**](https://github.com/LineageOS)
* [**Nitrogen Project**](https://github.com/nitrogen-project)
* [**ABC ROM**](https://github.com/ezio84)
* [**GZOSP**](https://github.com/GZOSP)
* [**Pure Nexus**](https://github.com/PureNexusProject)
* [**OmniROM**](https://github.com/omnirom/)
* [**AOSPA**](https://github.com/aospa/)
* [**BlissRoms**](https://github.com/BlissRoms)
* [**AOSPExtended**](https://github.com/AospExtended)

How to Build?(The following guide is write for Ubuntu 18.04 LTS)
-------------

To initialize your local repository using the ClickProject trees, use a 
command like this:

```bash
repo init -u https://github.com/CLickDev-Studio/Android -b oreo
```
  
Then to sync up:
----------------

```bash
repo sync -c -j4 --force-sync --no-clone-bundle --no-tags
```

If sync abort
-----------------
```bash
repo sync -c -j4 --force-sync --no-clone-bundle --no-tags
```

Before build
-----------------
Install the build packages
```bash
sudo apt-get install bc bison build-essential ccache curl flex g++-multilib gcc-multilib git gnupg gperf imagemagick lib32ncurses5-dev lib32readline-dev lib32z1-dev liblz4-tool libncurses5-dev libsdl1.2-dev libssl-dev libwxgtk3.0-dev libxml2 libxml2-utils lzop pngcrush rsync schedtool squashfs-tools xsltproc zip zlib1g-dev
```
Install openjdk-8-jdk
```bash
sudo apt-get install openjdk-8-jdk
```

Finally to build:

-----------------

```bash
  source build/envsetup.sh
  lunch aosp_device_codename-userdebug
  make cp -j4
```


Please do not forget to go through our website for technical support.
 
Chinese version/中文版本(大陆用户专用):[coding.NET](https://git.coding.net/Zecozhang/ClickProject_manifest_CN.git)





