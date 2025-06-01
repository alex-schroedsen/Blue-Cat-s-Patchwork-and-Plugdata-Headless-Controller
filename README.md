This is a program that I (Alex Schroedsen) wrote in order to operate Blue Cat's Patchwork and PlugData Standalone compiled with ASIO support in a headless manner for an embedded audio processing PC.

Parameters used to control this program:

BCP+PD_C.exe <1> <2> <3> <4> <5>

1: Set to 1 for 32-bit Blue Cat's Patchwork, 2 for 64-bit Blue Cat's Patchwork, 3 for Plugdata and 0 to suppress this message.

2: If running Blue Cat's Patchwork: Filename including extension also excluding path of a .preset file in %USERPROFILE%\Documents\Blue Cat Audio\Blue Cat's Patchwork\Presets to be applied.
If running PlugData: Filename including extension also including path of a .pd file.

3: Sampling rate to be applied in integer form.

4: Audio buffer size to be applied in integer form.

5: Audio Processing program process priority.
32             NORMAL_PRIORITY_CLASS
64             IDLE_PRIORITY_CLASS
128           HIGH_PRIORITY_CLASS
256           REALTIME_PRIORITY_CLASS
16384       BELOW_NORMAL_PRIORITY_CLASS
32768       ABOVE_NORMAL_PRIORITY_CLASS

Note: setting any of these parameters to 0 (Zero) will retain the current setting.
