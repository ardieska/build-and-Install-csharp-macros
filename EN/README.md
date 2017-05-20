# Build and Install

## Build Macro

You have to build the macro before you can use it in CorelDRAW:

1. Download and install [Visual Studio Community](https://www.visualstudio.com/free-developer-offers/).
1. Open Visual Studio (select _Visual C#_ environment in first run).
1. Change _Solution Configurations_ to _Release_ on Standard bar.
1. Build project (menu _Buil > Build {MacroName}_ / _Shift+F6_).

## Manual Installation

You can copy files manually without creating an installer:

1. Copy the macro _.\bin\Release\\{MacroName}.dll_ to _C:\Program Files\Corel\CorelDRAW Graphics Suite X7\Programs64\Addons\\{MacroName}_ (you need to create this folder).
1. Copy installer _.\installer\\{MacroName}Installer.gms_ to _C:\Users\\%your_user%\AppData\Roaming\Corel\CorelDRAW Graphics Suite X7\Draw\GMS_.

## Create Installer

Or you can create an installer for simple installation:

1. Download and install [Nullsoft Scriptable Install System](http://nsis.sourceforge.net/Main_Page).
1. Copy _.\bin\Release\\{MacroName}.dll_ to _.\installer_ folder.
1. Open context menu on _*.nsi_ file and select _Compile NSIS Script_.

After that you can install the macro by created _*.exe_ file.

## CorelDRAW

1. Run CorelDRAW.
1. Click _OK_ in the pop-up question. If you don't see it, open _Macro Manager_ or run _{MacroName}Installer_ manually.

After these actions macro's button appears on the _Standard Bar_.
