# Test core for Display Port, VGA, I2S sound and SCART (among other things)

This core presents a testcard, heavily based upon TVE testcard (nostalgia!). At the same time, a 1 kHz sine wave should be heard.

Image is present at the VGA port in both RGB 15 kHz (aka SCART mode), and industry standard VGA 640x480@60Hz mode, and Display Port (also 640x480).

At the bottom of the image, a series of hex numbers are shown: these are the current contents of DCDP registers, for debugging purposes. Current FPGA temperature is also shown in yellow characters.

This core is controlled by the keyboard:
- Key 1: switches between SCART mode and VGA mode (the default boot)
- Key 2: switches scanlines ON/OFF . Not visible in SCART mode.
- Key 3: cycle through the different monochrome modes: colour, green, amber and grayscale.
- Key 4: switches ON/OFF in-FPGA colour clock generation. Only valid if you have connected a PAL encoder to the VGA port.
- ESC  : exits core and return to ZX Spectrum core.
