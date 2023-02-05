# Schulze Method

[![Build status with Github Action][build-image-action]][build-action]
[![Code coverage][codecov-image]][codecov]
[![Code quality][codacy-image]][codacy]

This repository provides a Python implementation of the [Schulze method](http://en.wikipedia.org/wiki/Schulze_method).

## Requirements

- Install the latest version of [Python 3.X](https://www.python.org/downloads/) (at least version 3.10).

- Install the required packages:

```
pip install -r requirements.txt
```

## Usage

To rank candidates, import and call:

- either the `compute_ranks()` function, with [given signature](schulze.py#L90).

```python
from schulze import compute_ranks

schulze_ranking = compute_ranks(candidate_names, weighted_ranking_orders)
```

- or the `compute_schulze_ranking()` function, with [given signature](schulze.py#L106).

```python
from schulze import compute_schulze_ranking

schulze_ranking = compute_schulze_ranking(candidate_names, ballots)
```

<!-- Definitions -->

[build-action]: <https://github.com/woctezuma/schulze-method/actions>
[build-image-action]: <https://github.com/woctezuma/schulze-method/workflows/Python application/badge.svg?branch=master>

[pyup]: <https://pyup.io/repos/github/woctezuma/schulze-method/>
[dependency-image]: <https://pyup.io/repos/github/woctezuma/schulze-method/shield.svg>
[python3-image]: <https://pyup.io/repos/github/woctezuma/schulze-method/python-3-shield.svg>

[codecov]: <https://codecov.io/gh/woctezuma/schulze-method>
[codecov-image]: <https://codecov.io/gh/woctezuma/schulze-method/branch/master/graph/badge.svg>

[codacy]: <https://www.codacy.com/gh/woctezuma/schulze-method>
[codacy-image]: <https://api.codacy.com/project/badge/Grade/de8556d4681042c7ace2a1b95682be6b>
