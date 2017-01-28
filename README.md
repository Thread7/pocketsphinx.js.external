# pocketsphinx.js.external
pocketsphinx.js.external

This is a test of the https://github.com/syl22-00/pocketsphinx.js/ repository.  Specifically the part in the documentation where you try to load the acoustic model from external javascript files.  It is an attempt to recreate the pocketsphinx.js demo located at /webapp/live.html using the external model files.  The file /webapp/js/pocketsphinx.js was created using this command:

`cmake -DEMSCRIPTEN=1 -DCMAKE_TOOLCHAIN_FILE=c:\software\emcc\emscripten\1.35.0\cmake\Modules\Platform\Emscripten.cmake -G "MinGW Makefiles" -DHMM_EMBED=OFF ..`

pocketsphinx-default.js is the original from the original repository included for testing.




