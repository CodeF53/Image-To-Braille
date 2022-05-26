# Video To Braille
Covers a given video to a unicode version using braille characters and color escapes.

made for bad apple

## Basic Example
![Original](https://ia902905.us.archive.org/19/items/TouhouBadApple/Touhou%20-%20Bad%20Apple.mp4)

`py braille.py apple.mp4 --nocolor`

![After](https://cdn.discordapp.com/attachments/905438118746947687/979426343265644574/2022-05-26_10-49-29.mp4)

## Usage
```
usage: braille.py [-h] [-c C] [-s S] [--nocolor] [--irc] [--invert]
                  [--background BACKGROUND]
                  file

positional arguments:
  file                  The video file to render

optional arguments:
  -h, --help            show this help message and exit
  -c C                  The luma cutoff amount, from 0 to 255. Default 50
  -s S                  Size modifier. Default 1.0x
  --nocolor             Don't use color
  --irc                 Use IRC color escapes
  --invert              Invert the image colors
  --background BACKGROUND
                        The color to display for full alpha transparency
```

## Requirements
* python3
* [pillow](http://python-pillow.org/)
* [opencv](https://pypi.org/project/opencv-python/)