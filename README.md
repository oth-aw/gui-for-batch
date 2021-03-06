# Introduction

## Use this tool for batch-processing.

### Details

Works e.g. with

ffmpeg ffmpeg2theora

You can simply add some processing instructions to "converter.properties". Place e.g. ffmpeg (http://www.ffmpeg.org) , ffmpeg.exe ffmpeg2theora, ffmpeg2theora.exe or any other command-line-tool into the binaries-folder.

These instructions can be applied to one file or a complete folder. All files into this folder will be processed. Note: You can comment/uncomment with #

### Syntax:

```shell
(WIN | MAC) = <Command>;<Command>;...
<Command> ::= <Path-to-tool> <Options>, <Output-modifier>, <File-extension> 
```
### Example Windows:

```shell
WIN=binaries\\ffmpeg2theora.exe -v 4 -a 3,-o,_v4a3.ogg;binaries\\ffmpeg.exe -i,-b 64,_ffmpg.mpg
```
### Example Mac/Unix:

```shell
MAC=binaries/ffmpeg2theora -v 7 -a 3,-o,_v7a3.ogg;binaries/ffmpeg -i,-b 64,_ffmpg.mpg
```
