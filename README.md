# mustang-midi-bridge-win

This application enables any Windows computer to translate MIDI messages to the proprietary USB protocol used by Fender Mustang amplifiers.

It is porting of https://github.com/snhirsch/mustang-midi-bridge to Windows.

It is tested only under Windows 10 but there is no fancy requirements. It should works from XP to 10.

It is a simple to use command-line program. In most cases the following command is enough.

<code>mustang_midi 0 1</code>


# Run

- Download the 3 files included in <code>bin</code> folder
- Put in any local folder (no installation required)
- Connect your Fender Mustang amplifies via USB and power on it
- From Command Prompt run
  - <code>mustang_midi</code> to list the available MIDI interfaces/ports
  - <code>mustang_midi 0 1</code> to start listen to port 0 and MIDI channel 1.


# Compile

