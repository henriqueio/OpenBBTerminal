---
title: bench
description: This page discusses the 'bench' function, part of the OpenBB Terminal,
  which allows users to load benchmarks into their portfolio. It provides details
  on the parameters, method of application, and examples utilizing Python for portfolio
  management.
keywords:
- portfolio benchmark
- portfolio management
- portfolio load
- financial data
- portfolio operations
---

import HeadTitle from '@site/src/components/General/HeadTitle.tsx';

<HeadTitle title="portfolio.bench - Reference | OpenBB SDK Docs" />

Load benchmark into portfolio

Source Code: [[link](https://github.com/OpenBB-finance/OpenBBTerminal/tree/main/openbb_terminal/portfolio/portfolio_model.py#L93)]

```python
openbb.portfolio.bench(portfolio_engine: portfolio_engine.PortfolioEngine, symbol: str, full_shares: bool = False)
```

---

## Parameters

| Name | Type | Description | Default | Optional |
| ---- | ---- | ----------- | ------- | -------- |
| portfolio_engine | PortfolioEngine | PortfolioEngine class instance, this will hold transactions and perform calculations.<br/>Use `portfolio.load` to create a PortfolioEngine. | None | False |
| symbol | str | Benchmark symbol to download data | None | False |
| full_shares | bool | Whether to mimic the portfolio trades exactly (partial shares) or round down the<br/>quantity to the nearest number | False | True |


---

## Returns

This function does not return anything

---

## Examples

```python
from openbb_terminal.sdk import openbb
p = openbb.portfolio.load("openbb_terminal/miscellaneous/portfolio_examples/holdings/example.csv")
output = openbb.portfolio.bench(p, symbol="SPY")
```

---
