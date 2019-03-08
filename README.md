# emoji-extractor

> Extracts high-resolution emoji PNGs from `/System/Library/Fonts/Apple Color Emoji.ttc`

This is a small ruby script that extracts the Apple Color Emoji PNG Symbols from their corresponding system font located at `/System/Library/Fonts/Apple Color Emoji.ttc`.

The extracted assets will be placed in a subfolder of one called "images", for each resolution in their own folder. File system structure is as follows:

```
.
├── README.md
├── emoji_extractor.rb
└── images
    ├── 20x20
    ├── 21x21
    ├── 32x32
    ├── 40x40
    ├── 48x48
    ├── 64x64
    ├── 96x96
    └── 160x160
```



## Test

Make sure the font exists. The response should look like the second line:

```
$ file /System/Library/Fonts/Apple\ Color\ Emoji.ttc
/System/Library/Fonts/Apple Color Emoji.ttc: TrueType font collection data, 2.0, 2 fonts, at 0x20 TrueType Font data, 16 tables, 1st "OS/2"
```



## Usage

```
$ ruby emoji_extractor.rb
```
