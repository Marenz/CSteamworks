CSteamworks
=======

_CSteamworks_ is a C ABI Wrapper for Valve's Steamworks API. It relys heavily on automatic code generation.
The primary use case for _CSteamworks_ is to act as a buffer between a scripting language and C++ Interfaces.

* Author: [Riley Labrecque](https://github.com/rlabrecque)
* License: [MIT](http://www.opensource.org/licenses/mit-license.php)
* [Github Project](https://github.com/rlabrecque/CSteamworks)
* [Reporting Issues](https://github.com/rlabrecque/CSteamworks/issues)
* Currently supports Steamworks SDK v1.25


[![Support via Gittip](https://rawgithub.com/twolfson/gittip-badge/0.1.0/dist/gittip.png)](https://www.gittip.com/rlabrecque/)
[![Support via Paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=2QWKYXPRH6GJW)

Building
--------

To use _CSteamworks_ you must be a Steamworks developer.

* Download the Latest Steamworks SDK from the Steamworks Partner site.
* Copy `redistibutable_bin/` over from the Steamworks SDK into the root of this folder.
* Copy the `steam/` folder located in `public/` over from the Steamworks SDK into the root of this folder.
* Run CSteamworks.py which will generate the wrapper files into `wrapper/`
* Use the Makefile/Project files in `build/` to compile the dynamic libraries.

Limitations
-----------

* _CSteamworks_ was not intended to be used directly from C/C++ therefore it does not provide header files.
* _CSteamworks_ does not currently support ISteamAppTicket or ISteamGameCoordinator as they do not provide a global interface.