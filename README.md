# LSTM Music Generation with Pitch and Duration Modeling

This project implements a deep learning model using LSTM networks to generate music sequences by predicting both **pitch** and **duration**. The model is trained on MIDI data and outputs new compositions as MIDI files, which can be converted and played as audio.

## Features

- Dual-feature modeling of pitch and duration with embedding layers.
- Embedding layers for pitch and duration tokenization.
- Dual-output architecture: Predicts both pitch and duration.
- Support for temperature sampling for more creative outputs.
- Generates new MIDI files.

## Model

The model uses stacked bidirectional LSTM layers to learn temporal patterns in music sequences. Each training example consists of a sequence of tokens representing pitch and duration pairs.

## Dataset

This project uses a **subset of the [Monster MIDI Dataset](https://huggingface.co/datasets/projectlosangeles/Monster-MIDI-Dataset)**. All MIDI files were preprocessed to clamp durations to a fixed set and extract pitch/duration pairs.

## Output

- `generated_music.mid`: MIDI file of the generated sequence.
- [A sample of generated music can be found here](./sample/sample_1.mp3)

## Acknowledgements

- MIDI data sourced from a subset of the **[Monster MIDI Dataset](https://huggingface.co/datasets/projectlosangeles/Monster-MIDI-Dataset)**.
