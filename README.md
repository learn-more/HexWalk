![hexwalk](hexwalk/images/hexwalk64.png)
# HexWalk - Hex Editor/Viewer/Analyzer
 
HexWalk is an Hex editor, viewer, analyzer.

Based on opensource projects like qhexedit2,binwalk and QT.

It is cross platform and has plenty of features:

* Advanced Find (can find patterns in binary files based on HEX,UTF8,UTF16 and regex)
* Binwalk integration
* Entropy Analysis
* Hash Calculator
* Bin/Dec/Hex Converter
* Hex file editing
* Diff file analysis
* Byte Patterns to parse headers


## Screenshots

* Main page
![hexwalk gui](screenshots/hexwalk_gui1.png)

* Advanced Search
![hexwalk gui](screenshots/hexwalk_gui5.png)

* Entropy Calculator
![hexwalk gui](screenshots/hexwalk_gui2.png)

* Binary Analyzer
![hexwalk gui](screenshots/hexwalk_gui3.png)

* Hash Calculator
![hexwalk gui](screenshots/hexwalk_gui4.png)

* Diff Analysis
![hexwalk gui](screenshots/hexwalk_gui13.png)

* Binary Patterns for header parsing
![hexwalk gui](screenshots/hexwalk_gui15.png)

## Usage

HexWalk release executables are self-contained, you can use as-is.
Binwalk functionalities need Binwalk to be installed on the OS. For Linux OS simply install binwalk with your package manager (eg. sudo apt install binwalk). On Mac install with "brew install binwalk" or from sources following the instructions on Binwalk repository.

For more details about the usage go to the Wiki:

https://github.com/gcarmix/hexwalk/wiki


## Binwalk on Windows OS

For Windows, Binwalk support is experimental, it is done using a python helper file that launches the commands and must be on the same path of hexwalk.exe.
In order for binwalk support to work on Windows it is necessary to install Python and to install binwalk, at the moment of writing on windows it is supported up to binwalk 2.1.1, sources of binwalk_2.1.1 are supplied inside the binwalk_windows folder. To install it on Windows just run "python setup.py install".

EDIT:
from release 1.4.2 binwalk executables are included in the windows release folder, so it is just necessary to install Python on Windows, then the binwalk files are resolved automatically.

## Build
If you want to build from source just open hexedit.pro in QT Creator and build it.
It is possible also to build from command line (linux_build.sh script provided).

## Acknowledgments

Thanks to these projects:

* Binwalk - https://github.com/ReFirmLabs/binwalk

* QHexEdit2 - https://github.com/Simsys/qhexedit2

* QT5
