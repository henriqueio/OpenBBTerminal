---
title: whales
description: Learn how to utilise Whale Alert's API with OpenBB Terminal for tracking
  high value transactions on major blockchains. This page contains detailed information
  on how to implement and use this feature to retrieve both live and historical onchain
  data from various cryptocurrencies.
keywords:
- Whale Alert API
- blockchain transactions
- onchain data
- cryptocurrency
- major blockchains
- crypto whales
- high value transactions
- transaction tracking
- data retrieval
---

import HeadTitle from '@site/src/components/General/HeadTitle.tsx';

<HeadTitle title="crypto.onchain.whales - Reference | OpenBB SDK Docs" />

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

<Tabs>
<TabItem value="model" label="Model" default>

Whale Alert's API allows you to retrieve live and historical transaction data from major blockchains.

Source Code: [[link](https://github.com/OpenBB-finance/OpenBBTerminal/tree/main/openbb_terminal/cryptocurrency/onchain/whale_alert_model.py#L86)]

```python
openbb.crypto.onchain.whales(min_value: int = 800000, limit: int = 100, sortby: str = "date", ascend: bool = False)
```

---

## Parameters

| Name | Type | Description | Default | Optional |
| ---- | ---- | ----------- | ------- | -------- |
| min_value | int | Minimum value of trade to track. | 800000 | True |
| limit | int | Limit of transactions. Max 100 | 100 | True |
| sortby | str | Key to sort by. | date | True |
| ascend | str | Sort in ascending order. | False | True |


---

## Returns

| Type | Description |
| ---- | ----------- |
| pd.DataFrame | Crypto wales transactions |
---

</TabItem>
<TabItem value="view" label="Chart">

Display huge value transactions from major blockchains. [Source: https://docs.whale-alert.io/]

Source Code: [[link](https://github.com/OpenBB-finance/OpenBBTerminal/tree/main/openbb_terminal/cryptocurrency/onchain/whale_alert_view.py#L21)]

```python
openbb.crypto.onchain.whales_chart(min_value: int = 800000, limit: int = 100, sortby: str = "date", ascend: bool = False, show_address: bool = False, export: str = "")
```

---

## Parameters

| Name | Type | Description | Default | Optional |
| ---- | ---- | ----------- | ------- | -------- |
| min_value | int | Minimum value of trade to track. | 800000 | True |
| limit | int | Limit of transactions. Maximum 100 | 100 | True |
| sortby | str | Key to sort by. | date | True |
| ascend | str | Sort in ascending order. | False | True |
| show_address | bool | Flag to show addresses of transactions. | False | True |
| export | str | Export dataframe data to csv,json,xlsx file |  | True |


---

## Returns

This function does not return anything

---

</TabItem>
</Tabs>
