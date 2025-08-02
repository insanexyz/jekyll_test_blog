
### Tools used (learn and practice them seperately)
1. exif tool
2. cwebp
3. find

### Usage
1. Go recursively and remove exif data from all images and save them with same name
``exiftool -all= -r -overwrite_original .``

2. Change all images to webp with 80 percent of original image quality
``find . -type f \( -iname "*.jpg" -o -iname "*.png" \) -exec cwebp -q 80 {} -o {}.webp \;``