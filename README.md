# pynuvo-tuner
Python library for controlling Nuvo tuners (NV-T2SIR) via RS-232.

> **No longer maintained.** The driver now ships inside the [nuvo_tuner](https://github.com/brmccrary/nuvo_tuner) Home Assistant integration (1.2.0 and later), which no longer uses this library. The `nuvo-tuner` package stays on PyPI for older versions of the integration.

## Install

```
pip install nuvo-tuner
```

## Usage

```python
from nuvo_tuner import get_nuvo

nuvo = get_nuvo('/dev/ttyUSB0', '57600', 'seek')
model = nuvo.get_model()
status = nuvo.tuner_status('A')
```
