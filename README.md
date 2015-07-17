# celestia-g2-Qtsplash
 PLease  refer to https://github.com/bgodard/celestia-g2

## Note
Only use the gimp xcf from here if you want to improve the
celestia-g2.png splashscreen.
For the patched files and more continue at
https://github.com/raeTen/celestia-g2-stereoscopic
which contains these patches in a better manner.
Thanks.

## About
 This git contains a workaround for the disabled Qt splashscreen.
 Mainly I modified the old splash.png, which now
 also hopefully looks good with 1bit alpha-channeling instead of 8bit alpha.
 QPixmap.mask() will render 8bit alpha _with_ KDE-"desktop-effects"=on only,
 otherwise there's 1bit, which renders the old png in a "ugly" way.
 Call it a "bug", I don't know if or when this would be fixed.
 Works as designed, when you ask me...
 Normally we don't want desktop-effects on while using fps-orientated software
 like celesttia...
 The splash-ng is downward compatible, and could be used as splash.png
 for any older version, too.
 My patch will take the "splash-ng.png" for Qt. If your opinion says it's
 fancy enough, just use it.
 There are two or three pixels which probably disturb by a bright background,
 but hey, it's a splashscreen...
 So give it a try by using qtmain.cpp and qtappwin.cpp in src/celestia/qt and splash-ng.png
 in /celestia
 Another way would be having an own splash screen class like cel_splashscreen.cpp, 
 Due to less code, I'd prefer this way.

 Don't hesitate to "improve" the pixels, I added the gimp xcf ...
 