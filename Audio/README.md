# Extract Metadata

## Ffmpeg

ffmpeg can be used to check integrity of audio files and let it report infos and errors.

```
ffmpeg -v info -i [audio] -f null -
```

# Extract Embedded Data

## Wavsteg

WavSteg is a Python 3 tool that can hide data (using least significant bit) in wav files and can also extract data from them.

```
python3 WavSteg.py -r -b [lsb_number] -s [audio] -o [output]
```

## Sonic Visualizer

Sonic visualizer is a tool for viewing and analyzing the contents of audio files, however it can be helpful when dealing with audio steganography. You can reveal hidden shapes in audio files.

Link: https://www.sonicvisualiser.org/

## DeepSound

Run it and open the file and check if DeepSound finds any data hidden, in that case you will need to provide the password.

Link http://jpinsoft.net/deepsound/download.aspx
