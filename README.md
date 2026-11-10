# Ancapex B300 Price Index: reserved NVIDIA B300 rates

The weekly median of reserved NVIDIA B300 rates on terms of two years or longer that operators list publicly or allow us in writing to publish, in US dollars per GPU-hour, our fee included, with the quarters from which B300, GB300 NVL72, B200 and Vera Rubin can start in current offers.

- Live page, method and FAQ: https://www.ancapex.io/gpu-price-index
- Live CSV, updated every week (normally on Monday): https://www.ancapex.io/gpu-price-index.csv
- This repository: a copy of that file, last week in it: 26 October 2026.

On 10 November 2026 the B300 rates of every published week were withdrawn: they were counted from quotes operators sent us, and the index now counts only prices operators list publicly or allow us in writing to publish. The start dates stay. A week without enough such prices has empty rate columns.

## Columns of gpu-price-index.csv

| Column | Meaning |
| --- | --- |
| `week_of` | The week the figures describe (YYYY-MM-DD) |
| `b300_median_usd_per_gpu_hour` | Median of the B300 prices the week counts, USD per GPU-hour, our fee included; empty when not published |
| `b300_middle_half_low_usd`, `b300_middle_half_high_usd` | The middle half of those prices |
| `b300_priced_offers`, `b300_operators` | How many prices, and from how many operators, the week counts |
| `b300_start`, `gb300_nvl72_start`, `b200_start`, `vera_rubin_start` | The quarter from which operators in our pipeline can start each model; empty when not published that week |

## Method

The index counts prices for reserved NVIDIA B300 on terms of two years or longer that operators list publicly or allow us in writing to publish, and every figure comes from the prices of at least two operators.

Sample: B300 prices in US dollars for terms of two years or longer, received in the 30 days before the date, from operators' public price lists or from quotes an operator allows us in writing to publish. Prices operators share with us privately stay out, even in an aggregate. Resellers' offers are left out. Where an offer gives several terms we count its 3-year rate, or its shortest term of two years or longer when there is no 3-year rate. Every rate includes our fee. Figures are rounded to $0.10.

No figure from one operator: a rate is published only from 8 offers by 5 operators, with no operator above 40% of the offers, and every figure is computed from the prices of at least two operators. We show no lowest or highest offer. Until enough such prices are in, a model has no rate and the index shows start dates only.

The sample changes from week to week, so a change can come from a different mix of operators as well as from prices.

## Licence

CC BY 4.0, see `LICENSE`. Please credit: "Ancapex B300 Price Index, https://www.ancapex.io/gpu-price-index".

Questions: dima@ancapex.io
