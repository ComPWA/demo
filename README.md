# ComPWA demo notebooks

A collection of Jupyter notebooks that demonstrate features of the [ComPWA](https://github.com/ComPWA) packages [QRules](https://qrules.rtfd.io), [AmpForm](https://ampform.rtfd.io), and [TensorWaves](https://tensorwaves.rtfd.io). The notebooks are self-contained in the sense that they define their own pinned requirements and can be run independently in [Binder](https://mybinder.org) or [Google Colaboratory](https://research.google.com/colaboratory).

## Presentations

- **[2021.11.29](./2021.11.29)** [BESIII Collaboration Meeting Winter 2021](https://indico.ihep.ac.cn/event/15291)<br>
  [![Slides](https://img.shields.io/badge/view-slides-9cf?style=flat&logo=googledrive)](https://docs.google.com/presentation/d/e/2PACX-1vTMb3vsOqQUI_A3LYMs0iBvFwuIzyf49rG-PDXpR2TzwXJ4hkg-NzPB_Mslv7DcZuV1Tzm7duZEtI8q/pub)
  [![Binder](https://static.mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ComPWA/demo/main?urlpath=lab/tree/2021.11.29/qrules.ipynb)
  [![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ComPWA/demo/blob/main/2021.11.29/qrules.ipynb)

## Local installation

It's easiest to work with [Conda](https://docs.conda.io/en/latest/index.html) ([Miniconda](https://docs.conda.io/en/latest/miniconda.html)). The installation procedure then simply becomes:

```shell
conda env create
conda activate compwa-demo
pip install -r requirements.txt
pre-commit install
```

Style checks can now be performed with either of the commands `pre-commit run -a` or `tox`. To run a specific notebook or a folder with notebooks, use e.g.:

```shell
tox -e nb 2021.11.29/qrules.ipynb
```
