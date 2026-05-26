========================================================================
    Anthony : PlayStation1/2 Memory Card Utility
========================================================================
What is this software?
	This software reads and writes data from/to memory cards for Sony's home video game consoles, PlayStation 1 and 2, using a PC.
	It uses the Sony PlayStation 3 Memory Card Adaptor (CECHZM1) as the adaptor to read and write the memory cards.
	The supported memory cards are for PlayStation 1 and 2.
	
Supported OS
	Win8 or later
	From ver0.3.0.1 onwards, Win7 is no longer supported.
How to use
	First, install WinUSB as the driver for CECHZM1.
		Connect the CECHZM1 to a USB port, and when prompted to install the driver:
			"Browse my computer for drivers"
			"Let me pick from a list of available drivers on my computer"
			"Universal Serial Bus devices"
			Select "WinUSB Device" -> "WinUSB Device" in order, and install.

	Next,
	・If using a PS1 memory card, launch Anthony.exe.
	・If using a PS2 memory card, launch AnthonyPS2.exe.

		To read data from a memory card, click the "from Card" button.
		To read data from a file on the PC, click the "from File" button and select the file to read.

		To write data to a memory card, click the "to Card" button after reading data from either a memory card or a file.
		To save data to the PC, click the "to File" button and specify the save destination after reading data from either a memory card or a file.

	Supported Formats
		The supported file format for PS1 is the PSM format (128KB).
		The supported file format for PS2 is the PS2 format (8MB).

Motivation for Development
	Existing similar software has inconvenient aspects when used on Win7 or later.
	By releasing the source code, I intend to leave resources for future generations.

Development Environment
	As of Ver0.3.0.3:
		Visual Studio 2026 (18.6.1)
			Required additional installations:
			・C++ ATL for latest v145 build tools (x86 & x64)
			・MSVC v145 - VS 2022 C++ x64/x86 build tools (Latest)
Acknowledgments
	The code from jimmikaelkael's ps3mca-tool is used for reading and writing PS2 memory cards.