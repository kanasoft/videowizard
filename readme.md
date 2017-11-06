
Compiling KanaSoft VideoWizard

Windows

On Windows, you will need to install You can get Qt Creator from https://www.qt.io and the SDK included should already have everything you need :-) You need Qt 4.8 instead of the latest Qt 5.x since VideoWizard is also supported on older systems :-)
You can find the Qt version archives here:

https://download.qt.io/archive/qt/4.8/4.8.6/

Make sure you don't install it anywhere with spaces. We recommend you leave it at default. For this guide we're assuming your system drive is C:\, but substitute it for your letter if needed. Once installed, to make things easier, download the KanaSoft VideoWizard source from here by either Git pull, or ZIP. Copy it to the C:\QT\4.8.6 folder. Your directory structure should now look like:

C:\Qt\4.8.6\KanaVideoWizard-3.6.5\

Using the QT command Line, navigate to the folder by issuing the following command at the QT command prompt:

cd KanaVideoWizard-3.6.5

and then issue the follwing to build it:

qmake KanaSoftVideoWizard.pro && make

Linux Build Instructions

Compiling kanasoftvideowizard is really easy for Linux.

You will only need the Qt4 developer libraries in order to compile the program.
In addition, ffmpeg (no developer libs necessary) needs to be installed.

To compile kanasoftvideowizard, simply execute
qmake kanasoftvideowizard.pro && make

This will create an executable "kanasoftvideowizard" that you can start via ./kanasoftvideowizard.
