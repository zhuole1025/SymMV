# SymMV Dataset

[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

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