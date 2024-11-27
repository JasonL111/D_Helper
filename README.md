# D_Helper

## Description

This is a C program designed to organize and process `.LRF` files created by DJI devices. It provides the following functionalities:
- Create a directory named `LRF` and move all `.LRF` files into it.
- Rename all `.LRF` files in the `LRF` directory to have the `.MP4` extension.
- Compress all `.MP4` files in the `LRF` directory using the H265 codec and remove the original files that do not contain `_LRF` in their names.

## Why do we need it
Default LRF files use the H264 codec, which tends to be space-consuming. With this tool, you can compress them into smaller MP4 files using the H265 codec. This results in a more storage-efficient format that's also better optimized for streaming and playback.

## Instalation
1. Download the released exe file.
2. Download FFmpeg
3. Add the D_Helper.exe's path into your PATH environment variable.
4. Then you can use it.

## Usage
```
D_Helper
  --help: print help information
  -m: Create a directory named 'LRF' in the current directory and move all .LRF files into it.
  -t: Rename all LRF files in the 'LRF' directory to have an .MP4 extension.
  -c: Compress all MP4 videos in the 'LRF' directory using the H265 codec. After compression, delete the original videos that do not contain '_LRF' in their names.
```

## Notice
- You have to download FFmpeg to compress LRF
- The compressed video quality will be 3Mbps, audio quality will remain the same.