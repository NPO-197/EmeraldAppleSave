# EmeraldAppleSave
Bad Apple, but it's a pokemon emerald save file

### WARNING GAME **WILL** CRASH THE SOUND CHIP AND START MAKING A VERY LOUD SCREECHING NOISE ON LOAD, PLEASE MUTE OR LOWER VOLUME BEFORE STARTING THE SAVE!!!

Download the .sav file from releases

# How to use
Download the 'EmeraldApple.sav' save file from releases, then load the save file onto a US copy of pokemon Emerald using your GBA save backup method of choice.
Or you may load the save file using a GBA emulator like mGBA.
Then just boot the game, and select continue save option at the start. 
The corrupted save file will imeadiatly jump to the bootstrap code, loading the payload into iWRAM and executing the compiled binary, and start playing the video. 


## Build
To build the save you need to run SaveFileInject.py script with python.
To build the payload.bin / bootstrap.bin you will need to install gvasm https://github.com/velipso/gvasm and then run:
```
  gvasm make payload.gvasm -o build/payload.bin
  gvasm make bootstrap.gvasm -o build/bootstrap.bin
```
Note the compiled payload and bootstrap binaries have been included in this repo...

