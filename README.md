# Japanese OCR in Python

## Dependencies

- Python 3
- OpenCV >= 4
- Tesseract (see below)

### Tesseract

- Install `tesseract` 4.0
- Download `jpn_vert.traineddata` [here](https://github.com/tesseract-ocr/tessdata/blob/master/jpn_vert.traineddata)
- Copy `jpn_vert.traineddata` in `/usr/share/tessdata`
- Check with `tesseract --list-langs` that `jpn_vert` correctly appears

### Archlinux

```
pacman -S opencv tesseract-ocr-git tesseract-data-jpn
```

## How to use

```
./main.py examples/sample_page.jpg
```

Followed by:

```
./main.py examples/sample_page.jpg --ocr
```

