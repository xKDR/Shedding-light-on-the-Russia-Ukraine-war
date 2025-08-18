# Shedding Light on the Russia-Ukraine War: Reproducible Research

This repository contains all code, data, and resources required to reproduce the analysis and results from the paper "Shedding Light on the Russia-Ukraine War".

## Overview

- **Purpose:** Enable full transparency and reproducibility for the study of economic impacts of the Russia-Ukraine war using nighttime lights data.
- **Contents:** Jupyter/Colab notebooks, scripts, vector boundary data, and instructions for running the analysis in a cloud-based environment.

## Getting Started

1. **Google Colab Notebook**
   - Run the analysis directly in your browser using [Google Colab](https://colab.research.google.com/github/xKDR/Shedding-light-on-the-Russia-Ukraine-war/blob/main/reproducible_research.ipynb).
   - No manual installation required; all dependencies are handled in the cloud.

2. **Local Setup**
   - Clone this repository:
     ```bash
     git clone https://github.com/xKDR/Shedding-light-on-the-Russia-Ukraine-war.git
     ```
   - Install required packages (see `requirements.txt` if provided).
   - Download vector boundary data and satellite imagery as described in the notebook.

## Data


**Vector boundary data:**
The original vector boundary data was downloaded from [GADM.org](https://gadm.org/).

Due to computational and visualization challenges, the raw shapefiles required significant preprocessing:

1. For computation, Siberia and the Russian Far East were too large to be processed as single units, so these regions were subdivided.
2. For visualization, Russia's coordinate reference system (CRS) was changed to improve map clarity.
3. Chukotka Oblast crosses the anti-meridian in the original shapefile; we split this shape into multiple polygons for correct handling.

For these reasons, we provide the processed vector data in the `data/` folder of this repository.

**Satellite imagery:** Downloaded automatically by the notebook.

## Reproducibility

- All code and analysis steps are documented in the notebook.
- Plots and results are generated within the same environment for consistency.
- The computational environment is fully specified for cloud-based execution.

## Links

- [Google Colab Notebook](https://colab.research.google.com/github/xKDR/Shedding-light-on-the-Russia-Ukraine-war/blob/main/reproducible_research.ipynb)
- [Paper: Shedding Light on the Russia-Ukraine War](https://xkdr.org/paper/shedding-light-on-the-russia-ukraine-war)

## Citation

If you use this repository, please cite:

- Patnaik, A., Hande, R., Shah, A., Thomas, S. (2025). Shedding Light on the Russia-Ukraine War. [Link](https://xkdr.org/paper/shedding-light-on-the-russia-ukraine-war)

## License

This project is released under the MIT License.

---

For questions or contributions, please open an issue or pull request.
