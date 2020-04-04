# mustang-midi-bridge-win

This application enables any Windows computer to translate MIDI messages to the proprietary USB protocol used by Fender Mustang amplifiers.

It is porting of https://github.com/snhirsch/mustang-midi-bridge to Windows.

It is tested only under Windows 10 but there is no fancy requirements. It should works from XP to 10.

It is a simple to use command-line program. In most cases the following command is enough.

<code>mustang_midi 0 1</code>


# Run

- Download the 3 files included in <code>bin</code> folder
- Save them in any local folder (no installation required)
- Connect your Fender Mustang amplifies via USB and power on it
- From Command Prompt run
  - <code>mustang_midi</code> to list the available MIDI interfaces/ports
  - <code>mustang_midi 0 1</code> to start listen to port 0 and MIDI channel 1.


# Compile

You don't need to compile anything because we provide binary files. However if you want build it from scratch, contribute or customize something I used the following steps.

  - Download and install [Visual Studio 2019](https://visualstudio.microsoft.com/en/vs/) (any version). I used the free Community Edition.
  - During installation it is enough to select "Desktop Development with C++" option
  - Run Visual Studio 2019
  - Clone the git repository (everything you need is included)
  - Open the Solution file <code>mustang-midi-bridge-win.sln</code>

