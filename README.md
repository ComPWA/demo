# ComPWA demo notebooks

A collection of Jupyter notebooks that demonstrate features of the [ComPWA](https://github.com/ComPWA) packages [QRules](https://qrules.rtfd.io), [AmpForm](https://ampform.rtfd.io), and [TensorWaves](https://tensorwaves.rtfd.io). The notebooks are self-contained in the sense that they define their own pinned requirements and can be run independently in [Binder](https://mybinder.org) or [Google Colaboratory](https://research.google.com/colaboratory).

## Presentations

- **2021.09.08** [PWA 12 / ATHOS 7 in Bristol](https://indico.cern.ch/event/885396/contributions/4373645)<br>
  [![Slides](https://img.shields.io/badge/view-slides-9cf?style=flat&logo=googledrive)](https://docs.google.com/presentation/d/e/2PACX-1vQUqojagLjhMa_GQjQCTxCbtACwoDKwac9zoYorQrTZ3BF8cq9eJ349dF7nWzg1bS1oPL8NRbD-lGQx/pub)
- **2021.10.08** [LHCb Amplitude Analysis Meeting](https://indico.cern.ch/event/1081320)<br>
  [![Slides](https://img.shields.io/badge/view-slides-9cf?style=flat&logo=googledrive)](https://do?slide=id.pcs.google.com/presentation/d/e/2PACX-1vTUQRI34jbEG6MIXFHZiIYiXD0H2JFEUJTO5DEfDZjZNyHi6hQDTJy4URvMiyT-g0ENYP8dRsdnlrI_/pub)
- **[2021.11.29](./2021.11.29)** [BESIII Collaboration Meeting Winter 2021](https://indico.ihep.ac.cn/event/15291)<br>
  [![Slides](https://img.shields.io/badge/view-slides-9cf?style=flat&logo=googledrive)](https://docs.google.com/presentation/d/e/2PACX-1vTMb3vsOqQUI_A3LYMs0iBvFwuIzyf49rG-PDXpR2TzwXJ4hkg-NzPB_Mslv7DcZuV1Tzm7duZEtI8q/pub)
  [![Binder](https://static.mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ComPWA/demo/main?urlpath=lab/tree/2021.11.29/qrules.ipynb)
  [![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ComPWA/demo/blob/main/2021.11.29/qrules.ipynb)
- **[2021.12.13](./2021.12.13)** PANDA Seminar December 2021<br>
  [![Slides](https://img.shields.io/badge/view-slides-9cf?style=flat&logo=googledrive)](https://docs.google.com/presentation/d/e/2PACX-1vSymz5AjdhPw4Kz1pKhdFMnFGYuQvVaC8WbV_HTg770x6RDYoP-Anv9tn88DSuzvSiiQ9F4pcDGVExv/pub)
  [![Binder](https://static.mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ComPWA/demo/main?urlpath=lab/tree/2021.12.13/qrules.ipynb)
  [![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ComPWA/demo/blob/main/2021.12.13/qrules.ipynb)

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
