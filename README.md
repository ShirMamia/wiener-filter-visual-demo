# Wiener Filter Visual Demo

A Hebrew-language Jupyter notebook that explains frequency-domain Wiener filtering with a reproducible synthetic signal. It adds white noise to two sine waves, computes a frequency-dependent filter, and compares the reconstruction with the clean reference.

## Run locally

Use Python 3.11 or 3.12. In a virtual environment, install the dependencies and open the notebook:

```sh
python -m pip install -r requirements.txt
python -m notebook wiener_filter_visual_demo_hebrew.ipynb
```

Run all cells to generate 11 plots, including the clean and noisy signals, their spectra, the filter response, and the reconstruction error. The default seed gives the following results:

| Metric | Before filtering | After filtering |
| --- | ---: | ---: |
| Mean squared error | 0.958279 | 0.006007 |
| Signal-to-noise ratio | −1.86 dB | 20.17 dB |

The demo uses known clean-signal and noise spectra. For measured data, these spectra would need to be estimated or supplied in advance. The numbers above are specific to the synthetic example.

All input data is generated in the notebook. The notebook runs without data downloads or credentials.
