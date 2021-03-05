My patch for codeblocks 20.03 improves the Memory Dump dockable dialog.
I added a list box to it to select the number of columns to display.
Something like this is done in modern IDEs like AVR studio and other...
This is useful for debugging microcontrollers, viewing commands in 
their binary format, and more compact display of data.
Can select the following number of columns to display: 
2, 4, 6, 8, 10, 12, 14, 16, 18, 20, 22, 24, 26, 28, 30, 32. Also, the window will restore the position of the viewed data.

Svn version: 12293

Stable version:20.03

The patch works stably only if the font is set to more than 10 pt, change the line wxFont font (8, wxFONTFAMILY_MODERN, wxFONTSTYLE_NORMAL, wxFONTWEIGHT_NORMAL); the size you want in file examinememorydlg.cpp.

![Screenshot](/img/1.jpg)![Screenshot](/img/2.jpg)
![Screenshot](/img/3.jpg)
