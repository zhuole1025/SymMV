# SymMV Dataset

[![CC BY-NC-SA 4.0](https://camo.githubusercontent.com/7572a938f78b7dde0dbd741844b0b2bd7c031fdae63a420e0f80cbcd9911a154/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4c6963656e73652d434325323042592d2d4e432d2d5341253230342e302d6c69676874677265792e737667)](http://creativecommons.org/licenses/by-nc-sa/4.0/)

The SymMV dataset consists of annotations and musical representations corresponding to various music video URLs.

## Dataset Structure

```
SymMV/
│
├── SymMV.csv
│
├── chord/
│   ├── [filename1].chord
│   ├── [filename2].chord
│   └── ...
│
└── midi/
    ├── [filename1].midi
    ├── [filename2].midi
    └── ...
```

## Files & Directories Description:

- `SymMV.csv`: A tab-separated CSV file containing the following columns:
  - `index`: Unique identifier for each entry.
  - `youtube_url`: URL link to the music video.
  - `tonality`: Tonality of the corresponding music video.
  - `shazam_id`: An ID related to the Shazam platform. This ID can be used to search for corresponding song lyrics and metadata using the [shazamio](https://github.com/bogdanoff/shazamio) library.(e.g. `shazamio.shazam.track_about(shazam_id)`)

- `chord/`: This directory contains the chord annotations corresponding to each music video. The chord files have a `.chord` extension.

- `midi/`: This directory houses the MIDI representations for each music video. The MIDI files have a `.midi` extension.

## License

This dataset is licensed under the `CC BY-NC-SA` License. Please ensure you understand the licensing terms associated with this dataset before use. 