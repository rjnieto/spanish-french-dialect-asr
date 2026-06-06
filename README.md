# Spanish/French Dialect ASR Corpus

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.20575156.svg)](https://doi.org/10.5281/zenodo.20575156)

A 20-hour gender-balanced corpus of Spanish and French dialect speech with manual transcriptions.

## Data Access & Reproducibility

The audio segments are stored in a private Google Drive remote to comply with copyright restrictions on source material. Access is granted for research purposes only — redistribution of audio is not permitted.

To reconstruct the dataset:

1. Install DVC:
```bash
   pip install "dvc[gdrive]"
```
2. Clone this repo:
```bash
   git clone https://github.com/rjnieto/spanish-french-dialect-asr.git
   cd spanish-french-dialect-asr
```
3. Request Google Drive access by emailing: rjnieto@stanford.edu
4. Once access is granted, pull the audio:
```bash
   dvc pull
```

## Repository Contents

- `metadata.csv` — Manual transcripts, dialect labels, gender tags, and speaker IDs for 1,223 minutes of speech across 129 speakers
- `Audio Files.dvc` — DVC pointer to the audio corpus (hosted on private Google Drive)
- `.dvc/config` — Remote storage configuration


## Citation

```bibtex
@inproceedings{nieto2026_interspeech,
  title     = {Dialect Bias in Speech Recognition Across 10 Spanish and French Varieties},
  author    = {Nieto, Rodrigo and Angelika-Nikita, Maria and Sarkis, Diane and Yang, Diyi},
  booktitle = {Proceedings of Interspeech 2026},
  year      = {2026}
}
```

## Contact

For data access requests or questions, contact Rodrigo Nieto at rjnieto@stanford.edu.
