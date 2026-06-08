# homecastr-cookbook

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

**Ready-to-run notebooks for probabilistic real estate analysis with the Homecastr API.**

We're on a mission to make institutional-grade home value forecasting accessible to every analyst, quant, and developer. This cookbook open-sources our research workflows — from simple address lookups to multi-market investment screening.

---

## Prerequisites

**1. Get a free API key**

```python
from homecastr import HomecastrClient
result = HomecastrClient().keys.create("you@example.com")
print(result["key"])
```

Or sign up at [homecastr.com](https://www.homecastr.com). Store the key as `HOMECASTR_API_KEY` in your environment.

**2. Install the SDK**

```bash
pip install -U homecastr
pip install jupyter matplotlib h3  # for notebooks
```

---

## Examples

### Getting Started

| Notebook | Description |
|---|---|
| [Introduction to Forecasts](examples/getting_started/01_introduction.ipynb) | Your first address forecast — understanding P10/P50/P90 and reliability |
| [Bulk Address Lookup](examples/getting_started/02_bulk_lookup.ipynb) | Retrieve forecasts for a list of addresses and export to CSV |
| [Parcel Fan Chart](examples/getting_started/03_parcel_fan_chart.ipynb) | Download and visualize the full probability fan chart for a tax parcel |

### Neighborhood Analysis

| Notebook | Description |
|---|---|
| [H3 Neighborhood Heatmap](examples/neighborhoods/01_h3_heatmap.ipynb) | Map opportunity scores across Houston using H3 hex cells |
| [Cross-Market Comparison](examples/neighborhoods/02_market_comparison.ipynb) | Compare Houston · Austin · SF · NYC: 5-year outlook and proforma metrics |
| [Opportunity Ranking](examples/neighborhoods/03_opportunity_ranking.ipynb) | Screen and rank neighborhoods by risk-adjusted growth potential |

### Investment Analysis

| Notebook | Description |
|---|---|
| [DSCR Screening](examples/investment/01_dscr_screening.ipynb) | Filter properties by debt-service coverage ratio across a market |
| [Cap Rate Distribution](examples/investment/02_cap_rate_distribution.ipynb) | Analyze cap rate dispersion and identify underpriced submarkets |
| [Fan Chart Underwriting](examples/investment/03_fan_chart_underwriting.ipynb) | Use the P10/P90 spread to model upside/downside acquisition scenarios |

---

## License

MIT © Homecastr
