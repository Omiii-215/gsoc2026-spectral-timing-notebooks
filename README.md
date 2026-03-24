# GSoC 2026 — Spectral Timing in Julia (Stingray.jl) — Notebooks

> **Author:** Om Habib ([@Omiii-215](https://github.com/Omiii-215))
> **Project:** [Spectral Timing in Julia](https://github.com/StingraySoftware/Stingray.jl) — GSoC 2026, OpenAstronomy

This repository contains Jupyter notebooks demonstrating the **basic framework and implementation concepts** for my GSoC 2026 project: extending [Stingray.jl](https://github.com/StingraySoftware/Stingray.jl) with advanced spectral timing tools.

Each notebook implements the core analysis pipeline in **Python + [Stingray](https://docs.stingray.science/)** using simulated data, serving as a conceptual reference before porting each tool to Julia.

---

## 📓 Notebooks

| # | Notebook | Description |
|---|----------|-------------|
| 1 | [**Powerspectrum Framework**](01_powerspectrum_framework.ipynb) | `Powerspectrum` & `AveragedPowerspectrum` with Leahy, rms, and absolute normalizations |
| 2 | [**Crossspectrum, Time Lags & Coherence**](02_crossspectrum_time_lags_coherence.ipynb) | `Crossspectrum`, frequency-dependent time lags, and intrinsic coherence |
| 3 | [**Covariance & Lag-Energy Spectra**](03_covariance_lag_energy_spectra.ipynb) | Variability-vs-energy framework: covariance spectra and lag-energy spectra |
| 4 | [**Lomb-Scargle Periodogram**](04_lomb_scargle_periodogram.ipynb) | Periodograms for unevenly sampled / GTI-gapped data |
| 5 | [**NICER Data Analysis Demo**](05_nicer_data_analysis.ipynb) | End-to-end spectral timing pipeline on simulated NICER-like data |

---

## 🔧 Dependencies

```
pip install stingray numpy matplotlib astropy scipy
```

---

## 📚 References

- **Stingray documentation:** https://docs.stingray.science/
- **Stingray simulator:** https://docs.stingray.science/en/stable/simulator.html
- **NICER Data Analysis Workshop (Timing):** [heasarc.gsfc.nasa.gov](https://heasarc.gsfc.nasa.gov/docs/nicer/data_analysis/workshops/nicer_wkshp_timing_5_4_21.pdf)
- Huppenkothen, D., et al. (2019). *Stingray: A Modern Python Library for Spectral Timing.* ApJ, 881, 39.
- van der Klis, M. (1989). *Fourier Techniques in X-Ray Timing.* NATO ASI Series, 262, 27–69.
- Vaughan, B. A. & Nowak, M. A. (1997). *X-Ray Variability Coherence.* ApJ, 474, L43.
- Uttley, P., et al. (2014). *X-ray reverberation around accreting black holes.* A&A Rev., 22, 72.
- Scargle, J. (1982). *Studies in astronomical time series analysis. II.* ApJ, 263, 835.

---

## 🌟 GSoC 2026 Project Overview

This project extends Stingray.jl (the Julia port of Stingray) with:
1. **Powerspectrum / Crossspectrum types** — Leahy, rms, absolute normalization
2. **Time lags & coherence** — frequency-dependent lag extraction with bias correction
3. **Covariance & lag-energy spectra** — variability-vs-energy framework
4. **Lomb-Scargle periodograms** — for unevenly sampled data
5. **Comprehensive tests** — validated against Python Stingray
6. **Plot recipes & documentation** — publication-quality visualizations

---

*See also: [kashish2210/notebooks](https://github.com/kashish2210/notebooks) — GSoC 2025 reference notebooks*
