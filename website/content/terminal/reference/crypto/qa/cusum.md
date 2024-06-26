---
title: cusum
description: Learn about the Cumulative Sum Algorithm (CUSUM) used to detect abrupt
  changes in data. Understand its usage, parameters, and visualize how it works.
keywords:
- cusum
- cumulative sum algorithm
- data change detection
- usage of cusum
- parameters of cusum
- threshold
- drift
---

import HeadTitle from '@site/src/components/General/HeadTitle.tsx';

<HeadTitle title="crypto/qa/cusum - Reference | OpenBB Terminal Docs" />

Cumulative sum algorithm (CUSUM) to detect abrupt changes in data

### Usage

```python
cusum [-t THRESHOLD] [-d DRIFT]
```

---

## Parameters

| Name | Description | Default | Optional | Choices |
| ---- | ----------- | ------- | -------- | ------- |
| threshold | threshold | 0.0 | True | None |
| drift | drift | 0.0 | True | None |

![cusum](https://user-images.githubusercontent.com/46355364/154306207-d68f53f4-2f9a-4c1a-8e0e-b83d49938759.png)

---
