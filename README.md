# QTFiles - QuickTime Files for qaac QuickTime AAC encoder

Apple's [Core Audio AAC encoder](https://wiki.hydrogenaud.io/index.php?title=Apple_AAC) for [qaac](https://github.com/nu774/qaac).

This is the files required for qaac to encode without installing iTunes, QuickTime, or AppleApplicationSupport.msi.

Extracted directly from the latest iTunes installer using the [makeportable](https://sites.google.com/site/qaacpage/cabinet/makeportable.zip) script from the qaac's site.

## Installation

1. Download QTfiles (if you are using qaac.exe) or QTfiles64 (if you are using qaac64.exe).
2. Place the QTfiles folder if you are using qaac.exe or QTfiles64 folder if you are using qaac64.exe besides the qaac executable file.
3. Finished.

## Infos about the "icudt55.dll"
The "icudt55.dll" in the repo is just a [dummy file](https://hydrogenaud.io/index.php/topic,85135.msg907418.html#msg907418) because most of the content in the icudt55.dll is not required. But the original file is in the icudt55.7z. GitHub can't take files larger than 25MB so we compressed it.

"For encoding only, most of the content in the icudt55.dll is not required. But the file icudt55.dll can't be deleted, the encoder would refuse to work if it is not present. But you can replace the original files of several MB size with the tiny dummy DLL's, and the encoder still works." - LigH

### More Infos
[Using qaac without iTunes](https://github.com/wieslawsoltes/BatchEncoder/wiki/Tutorial-Using-qaac-without-iTunes)
