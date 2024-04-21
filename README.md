
<p align="left">
  <img src="https://github.com/Manut38/WLED-GifPlayer-html/assets/18471596/a6337fa6-70f5-4b9d-aac3-4766b5e13ba2" width="500px">
</p>

## WLED GIFPlayer

A WLED UI extension for an easy control of the awesome new "Image" effect, capable of displaying animated GIFs on your LED matrix.

It is using the ESP filesystem editor at `/edit` to list and change files on the local ESP storage.

## Features

- Click to change currently displayed image
- Upload/Delete image files
- Save images as presets
- Forced caching of images and request limiting (ESP crashes when there are too many concurrend HTTP requests)
- Button to refresh all images, useful when an image was replaced with another one of the same name

## Limitations

> [!WARNING]  
> **Only upload images in your matrix native resolution! (e.g. 16x16)**
> 
> Due to the limited flash storage space and processing power, .gif files of larger dimensions will make the effect lag and kill WLED performance

- Currently the "Image" effect only supports .gif files
- All image files will be uploaded to/read from the root path of WLEDs LittleFS because it does not support subfolders
- SD card support untested

# Installation

Download [gifplayer.htm](https://raw.githubusercontent.com/Manut38/WLED-GifPlayer-html/main/gifplayer.htm) and upload it to the WLED fileystem using `http://{WLED}/edit`

After that, the page can be accessed using `http://{WLED}/gifplayer.htm`

## Screenshots

![Screenshot Image List](https://github.com/Manut38/WLED-GifPlayer-html/assets/18471596/917093c2-f872-47a3-8b6c-8b92fa9de356 "Image select main screen")
![Screenshot Image Select](https://github.com/Manut38/WLED-GifPlayer-html/assets/18471596/81ac7234-062f-43ea-aff5-1ab5dac98019 "Right click/long press options")

## Footnotes

Thanks to [@ajotanc](https://www.github.com/ajotanc) for inspiring the layout and giving me a place to start using parts of his awesome [PixelMagicTool](https://github.com/ajotanc/PixelMagicTool)!

And of course, thank you [@Aircoookie](https://www.github.com/Aircoookie) and the entire WLED community for lighting up our homes! 🏠✨
