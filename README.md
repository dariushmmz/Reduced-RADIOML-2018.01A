# RadioML 2018.01A - Reduced Dataset

A reduced subset of the DeepSig RadioML 2018.01A dataset, created for faster
development and testing without downloading the full 18GB file.

## Source

Derived from the official RadioML 2018.01A dataset:
https://www.kaggle.com/datasets/pinxau1000/radioml2018

## Download

Reduced dataset (HDF5):
https://drive.google.com/file/d/1z4zsO2Tsv_KRE7BLlQ1knI8CTDNsvO4D/view?usp=sharing

## Contents

File: `DEEPSIG_2018_reduced.hdf5`

| Key | Shape | Type | Description |
|-----|-------|------|-------------|
| X | (N, 1024, 2) | float32 | I/Q samples per frame |
| Y | (N, 8) | int8 | One-hot modulation label |
| Z | (N, 1) | int64 | SNR in dB |

Total samples (N): 36,000

## Modulations included

- BPSK
- QPSK
- 8PSK
- 16QAM
- 64QAM
- GMSK
- AM-DSB-WC
- AM-DSB-SC

## SNR levels included (dB)

-10, -6, -2, 0, 2, 6, 10, 14, 18

## Samples per (modulation, SNR) pair

500

## Notes

- Same schema as the original dataset (X, Y, Z), only fewer rows.
- Modulation and SNR subsets were chosen for a specific project; edit the
  reduction script if you need different classes or SNR ranges.
- Not affiliated with or endorsed by DeepSig Inc. Refer to the original
  dataset license before redistributing.

## License

Same license terms as the original RadioML 2018.01A dataset apply.
