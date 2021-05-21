# Extract Metadata

## File

We can use the file command to identify the file type.

```
file [image]
```

## Exiftool

A much more advanced tool for extracting information from images is exiftool.

```
exiftool [image]
```

## Identify

You can also identify to check what kind of image a file is. Additionally, it checks if the image is corrupted.

```
identify -verbose [image]
```

# Extract Text

## Strings

Strings is a linux tool that displays printable strings in a file. Usually the embedded data is password protected or encrypted and sometimes the password is actaully in the file itself and can be easily viewed by using strings .

```
strings [file]
```

# Extract Embedded Data

## Steghide

Steghide is a steganography program that hides data in various kinds of image and audio files, only supports these file formats : JPEG, BMP, WAV and AU. 

Github Link: https://github.com/StefanoDeVuono/steghide

```
steghide info [image]
```

```
steghide extract -sf [image]
```

## Stegsolve

Sometimes there is a message or a text hidden in the image itself and in order to view it you need to apply some color filters or play with the color levels. It’s a small java tool that applies many color filters on images.

## Binwalk

Binwalk is a tool for searching binary files like images and audio files for embedded files and data.

Github Link: https://github.com/ReFirmLabs/binwalk

```
binwalk [image]
```

```
binwalk -e [image]
```


## Foremost

Foremost is a program that recovers files based on their headers, footers and internal data structures.

Github Link: https://github.com/korczis/foremost

```
foremost -i [image]
```

## Zsteg

`zsteg` is a tool that can detect hidden data in png and bmp files.

Github Link: https://github.com/zed-0xff/zsteg

```
zsteg -a [image]
```
