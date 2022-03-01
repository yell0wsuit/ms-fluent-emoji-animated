# Animated Microsoft Fluent Emojis (WIP)
Animated Microsoft Fluent emojis in WebP lossless format. This is a work-in-progress.

Taken from Developer Preview of Microsoft Teams.

<img src="https://raw.githubusercontent.com/yell0wsuit/ms-fluent-emoji-animated/main/webp/01%201f603_grinningfacewithbigeyes.webp">

This may appear as static on some browsers. Some of them may not appear anything at all.

## Supported browsers
- Google Chrome (desktop and Android) 32+
- Microsoft Edge 18+
- Firefox 65+
- Opera 19+

## Configuration
- GIMP with Python
- GIMP plug-ins: [ofn-layer-tiles](https://sourceforge.net/projects/gimp-tools/files/scripts/ofn-layer-tiles.zip/download), [Export Layer](https://github.com/khalim19/gimp-plugin-export-layers/releases)
- WebP lossless, export as animation, smaller output, delay for all frames 42 milliseconds.

## Guides (rough)
Very manual way, with a bit help from scripts.
- Open Microsoft Teams on the web, go to three dots near your avatar > About > Developer Preview. This might change the emoji appearance (for some), which you can right click and download emoji image.
- Install GIMP, then put plug-ins into ``%appdata%\GIMP\2.10\plug-ins``.
- Open emoji sprite you've downloaded in GIMP, then remove ".png" in the layer window (usually it's on the right).
- Change to RGB by Image > Mode > RGB.
- Go to Layer > Tiles > Split tiles (by width and height).
- Change the settings as follow (leave the Name as default) > OK:  
![](https://i.imgur.com/n8xqwff.png)
- Wait until it finishes extracting, then go to File > Export Layers... (recommend to choose a new empty folder, as it'll generate a lot of images). In File extenstion enter ``webp`` > Export. Tick only Lossless, and untick the rest > Export. Then wait.
- Close the image (you can use default shortcut <kbd>Ctrl</kbd> + <kbd>W</kbd>) > Discard Changes.
- Go to File > Open as Layers. Navigate to the folder where the images are generated in previous step, <kbd>Ctrl</kbd> + <kbd>A</kbd> to select all. Then wait.
- Go to File > Export As. Choose your favorite folder to export > Export. Use the following settings:  
![](https://i.imgur.com/iaM4J6e.png)
