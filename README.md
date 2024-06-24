# RedUtilities

A set of utitilies for making rocket league bots in C#

## Usage Instructions

### Prerequisites
Make sure you've installed [.NET SDK 6.0 x64](https://dotnet.microsoft.com/download),  
AND make sure you've installed [Python 3.7 64 bit](https://www.python.org/ftp/python/3.7.3/python-3.7.3-amd64.exe) or newer. During installation:
   - Select "Add Python to PATH"
   - Make sure pip is included in the installation
   

- Bot name, description, etc, is configured by `Bot.cfg`
- Bot strategy is controlled by `Bot/Bot.cs`
- Bot appearance is controlled by `Loadouts/loadout_generator.py`
- To make your bot run as fast as possible, build it in release mode, and then change the "executable_path" in `Bot.cfg` to `./Bot/bin/Release/net6.0/Bot.exe`
- See the [wiki](https://github.com/RLBot/RLBotCSharpExample/wiki) for tips to improve your programming experience.
- If you'd like to keep up with bot strategies and bot tournaments, join our [Discord server](https://discord.gg/q9pbsWz). It's the heart of the RLBot community!


## Overview of how the C# bot interacts with Python

The C# bot executable is a server that listens for Python clients.
When `python_run_file.py` is started by the RLBot framework, it connects to the C# bot server and tells it its info.
Then, the C# bot server controls the bot through the `RLBot_Core_Interface` DLL.

## Credit

-  [ddthj/GoslingUtils](https://github.com/ddthj/GoslingUtils) for inspiration on some of the structure and code (which I ported to c#)
-  [VirxEC/VirxERLU](https://github.com/VirxEC/VirxERLU) for the basis of my aerial code (which I ported to c#)
-  [Darxeal/BotimusPrime](https://github.com/Darxeal/BotimusPrime) for inspiration on some of the structure and driving code (which I ported to c#)
