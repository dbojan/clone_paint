# clone_paint
2026-10-16-09-39-35

Clone Paint — PyQt5 paint with a familiar interface

![alt text](screenshot.png)

requirements.txt:  
```
PyQt5>=5.6  
pillow
# JPEG XL Pillow fallback (used when the Qt JXL plugin is absent)  
pillow-jxl-plugin  
```
pip install -r requirements.txt

For jxl, if installed [qt-jpegxl-image-plugin](https://github.com/novomesk/qt-jpegxl-image-plugin) will be used, otherwise pillow will convert image temporarily from and to jxl.

For webp, if the Qt WebP plugin (qtimageformats qwebp) is installed it will be used, otherwise Pillow (built-in WebP support, no extra plugin) converts the image temporarily. 

WebP and JPEG XL save by default losslessly, or at quality 90 if 'Save JPEG XL/WebP lossless' is off.



Probably works on Windows, too.

### changes:

2026-10-16-09-39-35
- added support for webpy
- added File/New window command
- added checkbox for webp/jpegxl = save losless, on by default
- changed file save dialog to auto change file name extension (using qt file save dialog on all platforms)

2026-07-24-14-09-55
- added how to add 'open with Clone Paint' using xfce to readme.txt

2026-06-19-1
- added stamp tool

2026-06-02-1  
- bug fixes
