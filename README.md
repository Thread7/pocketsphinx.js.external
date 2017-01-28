# pocketsphinx.js.external
pocketsphinx.js.external

This is a test of the https://github.com/syl22-00/pocketsphinx.js/ repository.  Specifically the part in the documentation where you try to load the acoustic model from external javascript files.  It is an attempt to recreate the pocketsphinx.js demo located at /webapp/live.html using the external model files.  The file /webapp/js/pocketsphinx.js was created using this command:

`cmake -DEMSCRIPTEN=1 -DCMAKE_TOOLCHAIN_FILE=c:\software\emcc\emscripten\1.35.0\cmake\Modules\Platform\Emscripten.cmake -G "MinGW Makefiles" -DHMM_EMBED=OFF ..`

pocketsphinx-default.js is the original from the original repository included for testing.

You can test it here.
https://rawgit.com/Thread7/pocketsphinx.js.external/master/webapp/live.html

If you look in your browser console you will see this message:
`ERROR: "C:\inetpub\wwwroot-funder\bball\pockets\pocketsphinx\src\libpocketsphinx\acmod.c", line 79: Folder '' does not contain acoustic model definition 'mdef'`

Why would I get an error like this with the local path from my development machine?  

The files located in the /webapp/hub4js/ folder were taken from this repository: https://github.com/syl22-00/pocketsphinx.js-en_US-hub4wsj_sc_8k/
It seemed an easier way to get a test going than buld them myself.

If someone could give suggestions on how to get the loading of external files working, that would be great.



