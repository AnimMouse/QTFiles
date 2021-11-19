# QTFiles - QuickTime Files for qaac QuickTime AAC encoder

Apple's [Core Audio AAC encoder](https://wiki.hydrogenaud.io/index.php?title=Apple_AAC) for [qaac](https://github.com/nu774/qaac).

This is the files required for qaac to encode without installing iTunes, QuickTime, or AppleApplicationSupport.msi.

Extracted directly from the iTunes installer using the [makeportable](https://github.com/nu774/makeportable) script from the [qaac's site](https://sites.google.com/site/qaacpage/) using [GitHub Actions](https://github.com/features/actions).

## Installation

1. [Download](https://github.com/AnimMouse/QTFiles/releases) the latest QTfiles.7z (if you are using qaac.exe) or QTfiles64.7z (if you are using qaac64.exe).
2. Place the QTfiles folder if you are using qaac.exe or QTfiles64 folder if you are using qaac64.exe besides the qaac executable file.
3. Finished. qaac is now portable.

## icudt62.dll dummy file
The "icudt62.dll" inside the QTfiles.7z or QTfiles64.7z is just a [dummy file](https://hydrogenaud.io/index.php?topic=85135.msg977394#msg977394) because most of the content in the icudt62.dll is not required. But the original file is in the QTfiles64-icudt62.dll.zst or QTfiles-icudt62.dll.zst on the release.

"For encoding only, most of the content in the icudt55.dll (icudt62.dll) is not required. But the file icudt55.dll (icudt62.dll) can't be deleted, the encoder would refuse to work if it is not present. But you can replace the original files of several MB size with the tiny dummy DLL's, and the encoder still works." - [LigH](https://forum.doom9.org/showthread.php?p=1831215#post1831215)

Dummy DLL generated using [dummy-dll-generator](https://github.com/ykhwong/dummy-dll-generator).

## Microsoft Visual C++ Runtime
If you have it, no need to copy msvcp140.dll and vcruntime140.dll. If it's not working, install Visual C++ Redistributable for Visual Studio 2015 or download QTfiles-msvc.7z or QTfiles64-msvc.7z and place the dll besides the qaac executable file.

### Directory Tree

* For 32 bit
  * qaac.exe
  * QTfiles
    * ASL.dll
    * CoreAudioToolbox.dll
    * CoreFoundation.dll
    * icudt62.dll
    * libdispatch.dll
    * libicuin.dll
    * libicuuc.dll
    * objc.dll
* For 64 bit
  * qaac64.exe
  * QTfiles64
    * ASL.dll
    * CoreAudioToolbox.dll
    * CoreFoundation.dll
    * icudt62.dll
    * libdispatch.dll
    * libicuin.dll
    * libicuuc.dll
    * objc.dll

### More Infos
[Using qaac without iTunes](https://github.com/wieslawsoltes/BatchEncoder/wiki/Tutorial-Using-qaac-without-iTunes)

[Apple AAC](https://wiki.hydrogenaud.io/index.php?title=Apple_AAC)

[More Infos from hydrogenaudio](https://wiki.hydrogenaud.io/index.php?title=EAC_and_QAAC)

My recommended GUI encoder that can use qaac: [fre:ac](https://www.freac.org/)