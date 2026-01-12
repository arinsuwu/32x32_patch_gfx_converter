# 32x32 Patch GFX Converter
By Ari

## Description
This Python script convert a bulk player graphics file, usually in .bin format, used in Ladida's old [32x32 Player GFX patch](https://smwc.me/s/40241), into individual frame .bin files, used by Sonikku's new [32x32 Player GFX patch](https://www.patreon.com/posts/smw-patch-32x32-146703790).  
This allows you to keep using the old patch's file to, e.g. draw new frames over it using the included order as a reference, without having to go through the strain of having to copy each frame into its own, separate file.

## Usage
The script requires an install of Python to work. Run it as you would do any other script, or if you want to pass the graphics file as an argument, do `python ./convert.py <path_to_gfx_file>`. The output frames will be generated in a directory of the form `output_<gfx_file>`, each one a .bin file with a hex number filename in the same order as the old file, consisting of the format used in the new patch (one 32x32 frame and three dummy `X` tiles).