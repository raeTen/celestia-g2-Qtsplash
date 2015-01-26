# celestia-g2-Qtsplash
 PLease  refer to https://github.com/bgodard/celestia-g2
 
 This contains a workaround for the disabled Qt splashscreen.
 Mainly I modified the old splash.png, which now
 also hopefully looks good with 1bit alpha-channeling instead of 8bit alpha.
 QPixmap.mask() will render 8bit alpha _with_ KDE-"desktop-effects"=on only,
 otherwise there's 1bit, which renders the old png in a "ugly" way.
 Normally we don't want desktop-effects on while using fps-orientated software
 like celesttia...
 The splash-ng is downward compatible, and could be used as splash.png
 for any older version, too.
 My patch will take the splash-ng.png for Qt compiles. If you like it and find it 
 fancy enough like me, just use it.
 There are two or three pixels which probably disturb by a bright background,
 but hey, it's a splashscreen...
 So give it a try by using qtmain.cpp and qtappwin.cpp in src/qt and splash-ng.png
 in /celestia
 BTW, you don't need to do "make install" for testing purposes (Linux).