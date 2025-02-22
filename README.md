# crema
convolutional and recurrent estimators for music analysis

[![GitHub license](https://img.shields.io/badge/license-BSD-blue.svg)](https://raw.githubusercontent.com/bmcfee/crema/master/LICENSE)
[![Build Status](https://travis-ci.org/bmcfee/crema.svg?branch=master)](https://travis-ci.org/bmcfee/crema)
[![Coverage Status](https://coveralls.io/repos/github/bmcfee/crema/badge.svg?branch=master)](https://coveralls.io/github/bmcfee/crema?branch=master)
[![Documentation Status](https://readthedocs.org/projects/crema/badge/?version=latest)](http://crema.readthedocs.io/en/latest/?badge=latest)
[![Dependency Status](https://dependencyci.com/github/bmcfee/crema/badge)](https://dependencyci.com/github/bmcfee/crema)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1010486.svg)](https://doi.org/10.5281/zenodo.1010486)


Usage options
-------------

From the command-line, print to the screen in JAMS format:

```
python -m crema.analyze file.mp3
```

or save to a file:

```
python -m crema.analyze file.mp3 -o file.jams
```


From within python:

```python
from crema.analyze import analyze

jam = analyze(filename='/path/to/file.mp3', outputfile='optional/output/of/chroma/as/file.npy')
```

or if you have an audio buffer in memory, librosa-style:

```python
jam = analyze(y=y, sr=sr, outputfile='optional/output/of/chroma/as/file.npy')
```
