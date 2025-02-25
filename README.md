# BUILD STATUS
[![Build status](https://ci.appveyor.com/api/projects/status/mllnn7jx72ge8u6s/branch/master?svg=true)](https://ci.appveyor.com/project/BackTrak/allegiance)

# Installation

Download and install the latest "Visual Studio Community Edition" : https://www.visualstudio.com/downloads/

Download and install the latest Microsoft DirectX SDK (jun 2010): https://www.microsoft.com/en-us/download/details.aspx?id=6812 (if you don't want to install it, just extract the DirectX `include` and `lib` folders somewhere and set the environment variable `DXSDK_DIR` to their parent directory)

Launch Visual Studio and open the main solution `src\VS2022\Allegiance.sln`

There should be a prompt in the solution view to install required tools. If this is not the case, the installation will need to be modified.
This can be accessed from the installer, or from the Tab `Tools` -> `Get Tools And Features`.

## Required Tools
### Workloads
#### Desktop & Mobile
* .NET desktop development
* Desktop development with C++

### Individual Components
#### SDK's, libraries, and frameworks
* C++ MFC for latest v143 build tools (x86 & x64)

# Build
Once the solution, there is a button at the top to build. The configuration might need to change from `Debug` to `FZDebug`, `FZRelease`, or `Release`, if `Debug` does not build correctly.

# Main projects

* Allegiance (`WinTrek` folder) : the main client program
* Server (`FedSrv` folder) : the game server
* Lobby (`lobby` folder) : the game lobby
* IGC (`Igc` floder): game logic library

# Sub projects
* `zlib`: various low level libraries used by all projects
* `engine`: 3d gfx engine
* `effect`: fx engine above `engine`
* `clintlib`: client library
* `utility` (nb: folder name is _Utility) : various high level libraries used by the main projects (notably: network code and collision detection)
* `soundengine`: sound engine
* `training`: single player training missions 

# Obsolete (or about to be) projects
* AGC
* AllSrvUI
* AutoUpdate
* cvh
* mdlc
* reloader

# Links
* Forums: https://www.freeallegiance.org/forums/

* Discord : https://discord.gg/TXGmynB

* Kage Code Documentation: http://www.freeallegiance.org/FAW/index.php/Code_documentation

* Dropbox build instructions: https://paper.dropbox.com/doc/FreeAllegiance-build-instructions-LVrOqhj4PnD0UWkohmxmW

* Trello Bug Reports/Feature Request: https://trello.com/b/0ApAZt6p/steam-release-testing-dx9
