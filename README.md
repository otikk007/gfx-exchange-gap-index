# GFX.GE Exchange Gap Index (Georgia)

Daily open data on how much cash exchange rates differ across banks, microfinance organizations and exchange offices in Georgia.

- Live index and charts: https://gfx.ge/research/exchange-gap-index
- Latest CSV: https://gfx.ge/research/exchange-gap-index/data.csv
- Methodology: https://gfx.ge/methodology

This repository holds a snapshot. The live CSV on GFX.GE is the current source.

## Data

`gfx-exchange-gap-index.csv`, 36 daily rows from 2026-10-03 to 2026-11-07.

| Column | Meaning |
|---|---|
| `date` | Day, YYYY-MM-DD |
| `usd_index_pct` | Gap index for USD, percent of the official National Bank of Georgia rate |
| `eur_index_pct` | Gap index for EUR, percent of the official National Bank of Georgia rate |
| `usd_gap_gel_per_1000` | Lari gap on 1,000 USD: the average of the selling and buying gaps, rounded |

The first line of the file is a comment starting with `#`.

## Method

Index = (selling gap + buying gap) / 2, as a percent of the official rate. A gap is the difference between the best and the worst offer that day.

Excluded: rates not confirmed in the last 24 hours, rates where the buy rate is above the sell rate, and rates more than 5% away from the official rate. Card rates are a separate product and are not included. Rates can differ between branches; the main rate of each organization is used.

## License and citation

[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Please cite:

> GFX.GE, Exchange Gap Index, https://gfx.ge/research/exchange-gap-index

The data is informational and is not financial advice. Check the rate with the organization before you exchange.

## ქართულად

GFX.GE ყოველდღე ადარებს საქართველოს ბანკების, მიკროსაფინანსო ორგანიზაციებისა და გადამცვლელების ნაღდი ფულის კურსს. ეს ფაილი გაცვლის სხვაობის ინდექსის ასლია. ცოცხალი მონაცემები: https://gfx.ge/research/exchange-gap-index

მონაცემების გამოყენება შეგიძლიათ CC BY 4.0 ლიცენზიით, GFX.GE-ის წყაროდ მითითებით.
