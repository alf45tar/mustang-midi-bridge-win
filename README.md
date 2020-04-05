# mustang-midi-bridge-win

This application enables any Windows computer to translate [MIDI messages](/blob/master/doc/MIDX20_Midi_Spec.pdf) to the proprietary [USB protocol](/blob/master/doc/fender_mustang_protocol.txt) used by Fender Mustang amplifiers.

It is porting of https://github.com/snhirsch/mustang-midi-bridge to Windows.

It is tested only under Windows 10 but there is no fancy requirements. It should works from XP to 10.

It is a simple to use command-line program. In most cases the following command is enough.

<code>mustang_midi 0 1</code>

The complete MIDI implementation is [here](/blob/master/doc/MIDX20_Midi_Spec.pdf).

# Run

- Download the 3 files included in <code>bin</code> folder
- Save them in any local folder (no installation required)
- Connect your Fender Mustang amplifies via USB and power on it
- From [Command Prompt](https://www.howtogeek.com/235101/10-ways-to-open-the-command-prompt-in-windows-10/) run
  - <code>mustang_midi</code> to list the available MIDI interfaces/ports
  - <code>mustang_midi 0 1</code> to start listen to port 0 and MIDI channel 1.


# Compile

You don't need to compile anything because we provide binary files. However if you want build it from scratch, contribute or customize something I used the following steps.

  - Download and install [Visual Studio 2019](https://visualstudio.microsoft.com/en/vs/) (any version). I used the free Community edition.
  - During installation it is enough to select "Desktop Development with C++" option
  - Run Visual Studio 2019
  - Clone this github repository https://github.com/alf45tar/mustang-midi-bridge-win (everything you need is included)
  - Open the Solution file <code>mustang-midi-bridge-win.sln</code>

